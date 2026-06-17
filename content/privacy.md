---
# Privacy Policy

**Vital Scan Pro**
*Last Updated: March 22, 2025 | Version 1.0.0*
---
## Overview

Vital Scan Pro takes your privacy and the security of your health information very seriously. This Privacy Policy explains what data we collect, how we use it, how we protect it, and your rights under GDPR, HIPAA, CCPA/CPRA, and other applicable laws.

**If you are in the EU/EEA:** Mayco Lab LTD. acts as the **Data Controller** for your personal data.
**If you are in Turkey:** Processing is subject to **Turkish Law No. 6698 (KVKK)**.

---

## 0. Non-Medical Tool Classification

Vital Scan Pro is a **non-medical educational tool**. It is not a medical device as defined by the EU Medical Device Regulation (MDR) or Turkish Medical Device Regulations. The application provides AI interpretations of biomarkers for educational and historical tracking purposes only. It is not intended for the diagnosis, prevention, monitoring, or treatment of any physiological or pathological condition.

---

## 1. Information We Collect

### 1.1 Account Information

- Email address
- Display name (from Google sign-in or manually entered)
- Authentication credentials (managed by Firebase Auth — we do not store raw passwords)

### 1.2 Health Information (PHI)

- Blood test images and PDFs you upload
- Extracted biomarker values, units, reference ranges
- AI-generated analysis results and explanations
- Laboratory name and test date (if provided)

*All health information is classified as Protected Health Information (PHI) and is treated with the highest level of security.*

### 1.3 Usage Information (Non-PHI)

- App usage events (anonymised, no PHI included)
- Device type, operating system, app version
- IP address (for security and rate-limiting)
- Session duration

### 1.4 Payment Information

- Stripe processes all payments. Vital Scan Pro stores only your Stripe Customer ID — we never see or store full card numbers.

### 1.5 Location Information (Optional)

- Approximate location (only if you grant permission) to find nearby specialists
- We do not track your location continuously

---

## 2. Legal Basis for Processing (GDPR)


| Purpose                       | Legal Basis                         |
| ----------------------------- | ----------------------------------- |
| Providing the Service         | Contract (Art. 6(1)(b))             |
| Processing health data        | Explicit consent (Art. 9(2)(a))     |
| Security and fraud prevention | Legitimate interests (Art. 6(1)(f)) |
| Legal compliance              | Legal obligation (Art. 6(1)(c))     |
| Marketing (opt-in only)       | Consent (Art. 6(1)(a))              |

---

## 3. How We Use Your Information

- **Core Service**: OCR extraction, AI analysis, trend tracking
- **Security**: Fraud detection, abuse prevention, audit logging (HIPAA requirement)
- **Communication**: Service updates, analysis completion notifications
- **Billing**: Subscription management via Stripe
- **Legal Compliance**: HIPAA audit trails, GDPR compliance records (consent, deletion requests)
- **Product Improvement**: Aggregated, anonymised usage analytics only (never PHI)

**We do NOT:**

- Sell your personal or health data to third parties
- Use your PHI for advertising targeting
- Share PHI with insurers, employers, or government agencies without your consent (except as required by law)

---

## 4. Data Storage and Security

### 4.1 Encryption

- **At Rest**: All PHI is encrypted using AES-256. Files stored in AWS S3 with Server-Side Encryption (SSE-KMS). Database fields containing PHI are additionally encrypted at the application layer.
- **In Transit**: All data is transmitted over TLS 1.3.

### 4.2 Storage Locations

- Files: AWS S3 (US East) — HIPAA Business Associate Agreement in place
- Database: PostgreSQL (Supabase/AWS RDS) — HIPAA BAA in place
- Authentication: Firebase Auth (Google Cloud)

### 4.3 Access Controls

- Only you can access your health data
- Employee access is restricted to authorized engineers under NDA
- All PHI access is logged in our HIPAA audit trail

### 4.4 Retention

- Account data: Retained while your account is active + 30 days after deletion request
- Blood test files: Retained while your account is active, deleted within 30 days of your deletion request
- Audit logs: Retained for 6 years per HIPAA requirements (anonymised after account deletion)
- Consent records: Retained indefinitely for legal compliance (anonymised after account deletion)

---

## 5. Data Sharing and Third Parties

We share data with the following categories of third parties solely to provide the Service:


| Provider            | Purpose             | Data Shared           | Agreement |
| ------------------- | ------------------- | --------------------- | --------- |
| AWS (Amazon)        | File storage (S3)   | PHI files             | HIPAA BAA |
| Google Firebase     | Authentication      | Email, UID            | —        |
| Anthropic           | AI analysis         | Anonymised lab values | GDPR DPA  |
| Google Cloud Vision | OCR                 | Image content         | GDPR DPA  |
| Stripe              | Payments            | Email, billing info   | GDPR DPA  |
| Google Maps         | Location search     | Approximate location  | GDPR DPA  |
| SendGrid            | Email notifications | Email address         | GDPR DPA  |

All third-party processors are bound by appropriate Data Processing Agreements (DPAs).

### 5.1 AI Act Transparency (EU)

Per the EU AI Act, Vital Scan Pro is a **Limited Risk** AI system. Users are hereby notified that they are interacting with an AI (Gemini) for data analysis. This AI provides probabilistic interpretations and is not a medical professional.

*We do not use your data for AI model training without explicit opt-in consent.*

---

## 6. Your Rights

### 6.1 Rights under GDPR (EU/EEA Users)

- **Art. 15 — Right of Access**: Request a copy of all your personal data (`Settings → Export My Data`)
- **Art. 16 — Right to Rectification**: Correct inaccurate personal data via your profile settings
- **Art. 17 — Right to Erasure**: Request deletion of all your data (`Settings → Delete My Account`)
- **Art. 18 — Right to Restrict Processing**: Contact us at privacy@vitalscanpro.com
- **Art. 20 — Right to Data Portability**: Download your data in JSON format (`Settings → Export My Data`)
- **Art. 21 — Right to Object**: Object to processing based on legitimate interests
- **Right to Lodge a Complaint**: Contact your local supervisory authority

### 6.2 Rights under CCPA/CPRA (California Residents)

- Right to know what personal information is collected
- Right to delete personal information
- **Right to opt-out of the sale of personal information** (`Settings → Do Not Sell My Data`)
  - *We do not sell personal information. This opt-out is provided as a precautionary right.*
- Right to non-discrimination for exercising privacy rights

### 6.3 HIPAA Rights (US Users)

- Right to access your PHI
- Right to request amendment of your PHI
- Right to an accounting of disclosures of your PHI
- Right to request restrictions on use or disclosure of your PHI

### 6.4 Rights under KVKK (Turkey)

Turkish Data Subjects have the following rights under Art. 11 of Law No. 6698:

- Right to know if your data is processed
- Right to request information on the processing
- Right to know the purpose of processing
- Right to know the third parties to whom data is transferred (Section 5)
- Right to request correction or deletion
- Right to object to negative results of automated processing
- Right to claim compensation for damages due to unlawful processing

To exercise any rights, contact: **privacy@vitalscanpro.com**

We will respond within **30 days** (GDPR), **45 days** (CCPA), or as required by applicable law.

---

## 7. Children's Privacy

Vital Scan Pro is not intended for users under the age of 18. We do not knowingly collect personal information from children. If you are a parent and believe your child has provided us with personal information, please contact privacy@vitalscanpro.com immediately.

---

## 8. International Data Transfers

If you are located in the EU/EEA, your data may be transferred to the United States. We ensure adequate safeguards are in place through:

- Standard Contractual Clauses (SCCs) with US-based processors
- Data Processing Agreements with all third-party processors

---

## 9. Cookies and Tracking

**Mobile App**: We use minimal, privacy-respecting analytics only (no advertising trackers). Analytics events are anonymised — no PHI is included.

**Web App**: We use essential cookies for authentication sessions only. No advertising cookies.

---

## 10. Changes to This Policy

We will notify you of material changes via email and in-app notification at least 30 days before taking effect. Continued use after changes constitutes acceptance.

---

## 11. Contact Us

**Data Controller:** Mayco Lab LTD.
**Privacy Officer:** privacy@vitalscanpro.com
**Address:** str. Trajki Kitanchev, 4000 Plovdiv, Bulgaria
*This Privacy Policy was last reviewed by our legal team on March 22, 2025.*
----------------------------------------------------------------------------

Your privacy is important to us. This document outlines how we handle your data.

### Data Collection

We only collect what is necessary for the operation of VitalScan Pro.

### Data Security

All data is encrypted in transit and at rest.
