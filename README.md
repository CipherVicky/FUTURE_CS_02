# FUTURE_CS_02

## 🔍 Analysis Approach

The phishing email analysis followed a structured **7-step methodology** to ensure every email sample was examined consistently and accurately. This approach focuses on identifying phishing characteristics, assessing risk, and documenting findings in a professional manner.

### Step 1 — Collect Email Samples

Three phishing email samples were selected from publicly available educational repositories and security awareness resources. Each sample represents a different phishing technique commonly used by attackers.

| # | Attack Type | Psychological Trigger | Primary Goal |
|---|-------------|----------------------|--------------|
| 1 | Banking Account Verification | Fear — Account Suspension | Credential Theft |
| 2 | IT Support Password Reset | Authority — Corporate Request | Account Compromise |
| 3 | Prize / Lottery Scam | Greed — Unexpected Reward | Identity & Financial Theft |

---

### Step 2 — Analyse Email Headers

Each email header was reviewed to verify the authenticity of the sender and identify possible spoofing attempts.

The following header fields were examined:

- **From Address** — Verify whether the sender belongs to the legitimate organization.
- **Reply-To Address** — Check if replies are redirected to another email address.
- **Return-Path** — Compare with the sender's domain.
- **SPF Authentication** — Determine whether the sending server is authorized.
- **DKIM Signature** — Verify message integrity and authenticity.
- **DMARC Policy** — Check domain protection configuration.
- **Received Path** — Review mail server routing for anomalies.
- **Message ID** — Identify inconsistencies in message generation.

---

### Step 3 — Inspect Sender Domain & Embedded Links

All sender domains and URLs contained in the email were inspected for signs of deception.

| Technique | Example | Detection Method |
|-----------|---------|-----------------|
| Lookalike Domain | `secure-bank-login.net` | Compare with the organization's official domain |
| Typosquatting | `paypa1.com` | Inspect every character carefully |
| Subdomain Spoofing | `login.company.security-check.net` | Identify the actual registered domain |
| URL Shortener | `bit.ly/example` | Expand the URL before visiting |
| Free Hosting Abuse | `company-login.github.io` | Verify whether the organization owns the domain |
| Suspicious HTTPS Usage | Fake SSL Certificate | HTTPS alone does not guarantee legitimacy |

---

### Step 4 — Identify Phishing Indicators

Each email was evaluated against common phishing characteristics.

The primary indicators included:

1. Urgent or threatening language
2. Suspicious sender email address
3. Fake or misleading hyperlinks
4. Generic greeting (e.g., Dear User)
5. Grammar or spelling mistakes
6. Unexpected attachment
7. Request for passwords, OTPs, or confidential information

---

### Step 5 — Classify Email Risk

Each sample was classified according to the observed phishing indicators.

| Risk Level | Classification Criteria | Recommended Action |
|------------|------------------------|--------------------|
| 🔴 **PHISHING** | Multiple confirmed phishing indicators | Report immediately and avoid all interaction |
| 🟠 **SUSPICIOUS** | One or more questionable characteristics | Verify with the organization before responding |
| 🟢 **LEGITIMATE** | No phishing indicators detected | Safe to interact while maintaining normal vigilance |

The analysed email samples in this project were classified based on the identified indicators and overall risk level.

---

### Step 6 — Document Findings

Each email analysis was documented using a consistent reporting format.

The documentation includes:

- Email Subject
- Sender Information
- Screenshot of the Email
- Observed Phishing Indicators
- Risk Classification
- Technical Analysis
- Recommended User Actions

This standardized approach improves readability and makes comparisons between different phishing techniques easier.

---

### Step 7 — Security Awareness & Prevention

Based on the analysis, practical recommendations were prepared to help users recognize and avoid phishing attacks.

#### Employee Best Practices

- Verify the sender before responding.
- Hover over hyperlinks before clicking.
- Never share passwords or OTPs through email.
- Avoid opening unexpected attachments.
- Report suspicious emails to the IT Security Team.
- Enable Multi-Factor Authentication (MFA).

#### Organizational Security Controls

- Deploy SPF, DKIM, and DMARC.
- Conduct regular phishing awareness training.
- Enable Email Security Gateways.
- Perform periodic phishing simulation exercises.
- Monitor suspicious login attempts.
- Enforce Multi-Factor Authentication across critical services.

---

## 📊 Key Findings Summary

- ✅ Every analysed phishing email relied on **social engineering** to manipulate the recipient.
- ✅ **Urgency and fear** were the most frequently used psychological tactics.
- ✅ Spoofed sender domains and misleading URLs were present in the majority of samples.
- ✅ Requests for sensitive information such as passwords and OTPs remain a primary phishing objective.
- ✅ Verifying sender identity and inspecting URLs before clicking can prevent most phishing attacks.
- ✅ Combining **user awareness**, **email authentication (SPF, DKIM, DMARC)**, and **Multi-Factor Authentication (MFA)** significantly reduces the risk of successful phishing attacks.
- ✅ The strongest defence against phishing continues to be an informed and security-aware user.
