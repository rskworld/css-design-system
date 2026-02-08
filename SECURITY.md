# Security Policy

<!--
  © 2026 RSK World | https://rskworld.in
  Founder: Molla Samser
  Email: help@rskworld.in | support@rskworld.in
  Phone: +91 93305 39277
  Address: Nutanhat, Mongolkote, Purba Burdwan, West Bengal, India, 713147
-->

## Supported versions

| Version | Supported          |
| ------- | ------------------ |
| 1.x     | :white_check_mark: |

## Reporting a vulnerability

If you believe you have found a security vulnerability in this project:

1. **Do not** open a public issue.
2. Email **help@rskworld.in** or **support@rskworld.in** with:
   - Description of the vulnerability
   - Steps to reproduce (if possible)
   - Impact and suggested fix (optional)

We will acknowledge receipt and work with you to understand and address the issue.

## Scope

This project is a **CSS design system** (styles and demo HTML). It does not run server-side code or handle user credentials. Vulnerabilities of interest include:

- CSS that could be used to exfiltrate data or deceive users (e.g. phishing-style styling)
- XSS or injection risks in demo HTML/JS if reused in a vulnerable way

General best practice: always sanitize user input and use CSP where applicable when embedding or extending this system.

## Contact

- **RSK World:** https://rskworld.in  
- **Email:** help@rskworld.in | support@rskworld.in  
- **Phone:** +91 93305 39277  

---

© 2026 RSK World. All rights reserved.
