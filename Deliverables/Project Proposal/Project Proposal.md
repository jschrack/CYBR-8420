# CYBR-8420 Project Proposal

## Team Members
- Augusto Zorrilla Mendez
- Deb Peterson
- Geoff Humphreys
- Jesse Schrack
- Mark Magno



---

## Link to Project Board
[Click here to view the board](https://github.com/users/ghumphr/projects/1/views/1)

---

## Operational Environment

### Diagram of Operational Environment

---

## Motivation

---

## Software Description

---

## Licenses, Agreements, and Contributing

### License

**GNU AFFERO GENERAL PUBLIC LICENSE (AGPL)-3.0, Version 3, 19 November 2007**

[Copyright © 2007 Free Software Foundation, Inc.] (http://fsf.org/)

This is a free, copyleft license for software specifically designed to ensure cooperation with the community. General Public Licenses assert copyright on the software and give you permission to copy, distribute, and/or modify the software.

### Contributing

**Contributor License Agreement**

All contributors must sign a contributor license agreement (CLA) before pull requests will be accepted. Once a pull request is submitted, a status check will indicate whether a signature is still required or not. If the check fails, click on Details and complete the form. The CLA check on the pull request should be successful upon completion of the web form.

**Contributor Code of Conduct**

Contributions can be made to Canvas through filing issues or submitting pull requests. To ensure a respectful, harassment-free experience for contributors and maintainers of this project, any inappropriate material will be removed, edited, or rejected. Examples include sexual language or imagery, derogatory comments, harassment, or other unprofessional behavior. Incidents may be reported by contacting the project maintainers or through opening an issue.

---

## Security-related History For The Software

Canvas LMS has faced several security issues over the years. Some notable issues that were listed in Instructure’s Penetration Test Results report in May 2020 [Instructure Past Security Issues] (https://www.instructure.com/sites/default/files/file/2021-01/Instructure-Penetration-Test-Results-May-2020.pdf) include:

- **Critical (Priority 1)**
  - Leak of app Authorization token via Image with data-api endpoint (Sensitive Data Exposure)
  - ePortfolio export will bypass all access controls for files (Broken Access Control)
- **High (Priority 2)**
  - XSS in Group Wiki Pages via Prerequisites lookup exploit (Cross-Site Scripting)
  - Access to submission/comments media (Broken Access Control)
- **Medium (Priority 3)**
  - CSS in Canvas Quizzes via malicious response from server (Cross-Site Scripting)
  - Users can see automatically graded scores on muted or hidden assignments (Server Security Misconfiguration)
- **Low (Priority 4)**
  - Open Redirect (Unvalidated Redirects and Forwards)
  - Course members without permission to view grades can download all quiz submissions (Broken Access Control)
 
Canvas LMS participates in a bug bounty program through Bugcrowd, Inc. and has addressed the above listed security issues through the release of patches and updates. Instructure performs application assessment and penetration testing annually using an Ongoing Bounty Program to identify and mitigate security vulnerabilities.

---

## Reflections
---
