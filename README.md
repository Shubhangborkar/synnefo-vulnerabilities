# Synnefo Internet Management Software (IMS): Security Advisories

Coordinated-disclosure advisories for vulnerabilities found in **Synnefo Internet Management Software (IMS)**, a subscriber-management, billing and accounting platform used by internet service providers. Each file is the public reference for one CVE record.

| CVE | Advisory | Weakness | Severity* | CVE status |
|---|---|---|---|---|
| CVE-2022-45676 | [IDOR exposes bills and payment history](CVE-2022-45676-idor-billing-history.md) | CWE-639 | 6.5 Medium | Reserved, publication requested |
| CVE-2022-46617 | [SQL injection in the usage-details filter](CVE-2022-46617-sqli-usage-details.md) | CWE-89 | 8.8 High | Reserved, publication requested |
| CVE-2023-37774 | [Login with username and phone number only](CVE-2023-37774-login-without-password.md) | CWE-287 | 9.1 Critical | Reserved, publication requested |
| CVE-2023-37775 | [IDOR in the user-details API leads to account takeover](CVE-2023-37775-idor-user-details.md) | CWE-639 | 8.1 High | Reserved, publication requested |
| CVE-2023-37777 | [SQL injection in the payment-processing API](CVE-2023-37777-sqli-payment-api.md) | CWE-89 | 9.8 Critical | Published (22 Jan 2025) |

\* The CVE-2023-37777 score is the one listed for the published record. The other scores are the researcher's CVSS v3.1 assessments and will be replaced by NVD scores once those records are published.

## Disclosure Summary

- **First vendor contact:** 10 Nov 2022
- **Vendor acknowledgement:** 30 Jun 2023. On 05 Jul 2023 the vendor said patches were being rolled out to client servers in phases and asked for 45–60 days.
- **Coordination support:** CERT-In was contacted on 24 Jun 2023 to help reach the vendor.
- **Public disclosure:** more than three years after first contact, well past the standard 90-day window and the extensions the vendor asked for.

## Guidance for Operators

If you run Synnefo IMS, ask the vendor to confirm that your instance has the fixes for all five CVEs. Then rotate the database, payment-gateway, SMTP and SMS-provider credentials, and reset subscriber and administrator passwords.

## Responsible Disclosure Notes

- Exploit payloads, endpoint paths, customer domains and any customer data have been removed on purpose.
- All testing was done on the researcher's own subscriber account, with no more access than needed to confirm each issue.

## Reporter

Shubhang Borkar: [LinkedIn](https://www.linkedin.com/in/shubhangborkar) · [Medium](https://shubhangborkar.medium.com)

## License

[MIT](LICENSE)
