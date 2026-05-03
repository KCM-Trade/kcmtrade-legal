---
layout: default
title: Application Access Disclosure
effective_date: 27 January 2026
last_updated: 3 May 2026
---

This Application Access Disclosure (the “Disclosure”) sets out information regarding access to applications and digital services operated under the **KCM Trade** brand by **Kohle Capital Markets Limited** (the “Company”, “we”, “us”, or “our”).

This Disclosure is provided for transparency and to facilitate review by platform operators, regulators, and authorised reviewers, including but not limited to mobile application distribution platforms.

---

## 1. Scope of Application

This Disclosure applies to all mobile applications, web-based applications, and digital services operated, published, or distributed under the KCM Trade brand, whether accessed via:

- Apple App Store  
- Google Play Store  
- Huawei AppGallery  
- Web platforms  
- Application programming interfaces (APIs)  
- Embedded or integrated services  

---

## 2. Account-Based Access

Certain features of the Services may be accessible only to registered users with an active account.

Account creation may require the submission of personal information and completion of identity verification procedures in accordance with the Company’s **Privacy Policy**, **AML and KYC Policy**, and **Terms of Service**.

---

## 3. Access Restrictions

Access to the Services may be restricted based on, without limitation:

- Regulatory or legal requirements  
- Jurisdictional limitations  
- User eligibility criteria  
- Completion of required verification procedures  

The Company reserves the right to restrict or deny access to any user where required to comply with applicable laws, regulations, or platform policies.

---

## 4. Reviewer Access for Platform Assessment

For the purposes of application review by platform operators (including Apple App Store, Google Play Store, Huawei AppGallery, and other authorised distribution platforms), access to the Services may be provided through one or more of the following methods:

- Dedicated test or review accounts  
- Guided access workflows  
- Explanatory documentation outlining access procedures  
### 4.1 Demo Account Availability

The Company provides pre-verified demo (paper trading) accounts for use by platform reviewers. Demo accounts allow access to the application's core features — including account dashboard, trading interface, copy trading, signals, and education content — without the use of real funds or exposure to live markets.

Demo account credentials for reviewer use are available upon request and will be supplied directly to the relevant platform review team through the official review submission process.

### 4.2 Technology Infrastructure

The KCM Trade application is built on and integrates the following technology components:

| Component | Provider |
|---|---|
| Trading platform | MetaQuotes MT4 / MT5 and Leverate |
| CRM and back-office | FX Back Office (FXBO) |
| Identity verification (KYC) | ShuftiPro |
| Copy trading | Pelican Trading |
| Signals and education | Acuity Trading |
| Live support chat | Convrs.io |
| Website hosting | Webflow (via Cloudflare DNS) |
| Push notifications | OneSignal; Firebase Cloud Messaging (FCM) |
| Mobile attribution and analytics | AppsFlyer |
| Transactional email (OTP delivery) | SendGrid / Amazon SES (SMTP fallback) |
| Social registration authentication | Google Sign-In; Apple Sign-In (iOS); Microsoft MSAL |
| Address verification (KYC) | Google Maps Platform |

### 4.4 Device Permissions

The KCM Trade application requests the following device permissions at runtime. Each permission is requested only when required for the relevant functionality:

| Permission | Purpose | Platform(s) |
|---|---|---|
| **Camera** | QR code scanning for partner referral links; document photo capture for KYC upload | iOS, Android, Huawei |
| **Photo Library / Media Storage** | Image and document selection for KYC verification and file upload | iOS, Android, Huawei |
| **Location (approximate)** | Country geo-check at app launch to determine applicable CRM server and enforce jurisdictional access restrictions | iOS, Android, Huawei |
| **Biometrics (Face ID / Touch ID / Fingerprint)** | App lock authentication and quick login — biometric data is processed locally on-device and is not transmitted externally | iOS, Android, Huawei |
| **Push Notifications** | Account alerts, transaction status updates, and platform communications | iOS, Android, Huawei, Web |
| **App Tracking Transparency (ATT)** | iOS-only consent prompt required before AppsFlyer attribution tracking is activated | iOS only |

### 4.3 KYC-Gated Features

Certain features, including live trading, deposits, and withdrawals, are restricted to users who have completed identity verification in accordance with the Company's AML and KYC obligations. This restriction exists to comply with the requirements of the Financial Services Commission of Mauritius and applicable financial crime prevention laws. Demo accounts provided for review purposes are pre-verified and are not subject to these restrictions.Where live account access is not appropriate due to regulatory, security, or compliance considerations, sufficient information will be provided to enable a meaningful review of the application’s functionality.

---

## 5. Security and Compliance Considerations

In order to protect users, the integrity of the Services, and compliance with regulatory obligations, the Company may:

- Limit reviewer access to non-production or restricted environments  
- Mask or restrict access to sensitive data  
- Disable certain transactional or financial functionalities  

Such measures are implemented to ensure compliance with financial regulations, data protection laws, and security standards.

---

## 6. No Waiver of Legal or Regulatory Obligations

Nothing in this Disclosure shall be construed as:

- A waiver of any legal or regulatory obligation  
- A grant of unrestricted access to the Services  
- An entitlement to bypass security, compliance, or verification requirements  

All access remains subject to applicable laws, regulations, and contractual terms.

---

## 7. Amendments

The Company may amend this Disclosure from time to time to reflect changes in:

- Legal or regulatory requirements  
- Platform review policies  
- Operational or security considerations  

Any amendments shall take effect upon publication, as indicated by the updated **Last Updated** date.

---

## 8. Contact Information

For enquiries relating to application access or review procedures, please contact:

**Kohle Capital Markets Limited**  
Email: support@kcmtrade.com  
Website: https://www.kcmtrade.com  

---

This Disclosure forms part of the Company’s legal and compliance documentation and should be read in conjunction with other applicable policies and disclosures.
