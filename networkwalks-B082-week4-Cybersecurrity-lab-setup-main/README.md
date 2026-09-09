
# Mediroza – Web Application Penetration Testing

## Overview

This project documents a multi-phase penetration testing assessment conducted against the **Mediroza application** as part of a cybersecurity assessment.

The objective was to evaluate the application's security controls and determine whether sensitive patient and organizational information could be accessed through identified security weaknesses.

> **Disclaimer:** This project was conducted in an authorized testing environment for educational and cybersecurity assessment purposes only. The techniques and findings described here should only be applied to systems where explicit authorization has been provided.

---

## Assessment Objectives

The assessment focused on:

- Evaluating access control mechanisms
- Testing the protection of sensitive patient information
- Assessing the security of password-protected documents
- Identifying exposure of confidential organizational information
- Documenting security findings and their potential impact

---

## Assessment Phases

### Module 1 – Access Control Assessment

During the first phase, testing identified a weakness in the application's access control mechanisms.

The weakness allowed access to the **patient report functionality**, which should have been restricted to authorized users.

**Key Outcome:**
- Access to patient report functionality was successfully demonstrated.
<img width="958" height="401" alt="m1" src="https://github.com/user-attachments/assets/7a8d9365-79f4-4d74-91c8-3787876b4e73" />

---

### Module 2 – Protected Patient Reports

The second phase focused on patient reports containing sensitive information.

The reports were stored as **password-protected PDF documents**. During testing, weaknesses in the protection mechanism were identified, allowing access to **three patient reports** within the authorized assessment environment.

**Key Outcome:**
- Three protected patient reports were successfully accessed.
- The findings demonstrated weaknesses in the protection of sensitive patient information.
<img width="887" height="427" alt="mmm2" src="https://github.com/user-attachments/assets/7f5efbb7-5556-4ee8-b3cf-9a0a55fc0aa0" />
<img width="606" height="396" alt="mm2" src="https://github.com/user-attachments/assets/2eca69e7-f646-497c-afa1-0f459567b02c" />
<img width="433" height="305" alt="m2" src="https://github.com/user-attachments/assets/5c36fe19-a997-4d5b-bfdf-5ff299429084" />

---

### Module 3 – Sensitive Organizational Information

The final phase focused on identifying exposure of sensitive internal business information.

Testing resulted in access to:

- Staff salary information
- Stakeholder details

**Key Outcome:**

The findings demonstrated that sensitive organizational information was not sufficiently protected within the assessed environment.
Extracted the hidden information and using that clue in comments , found the /old repository.
<img width="626" height="271" alt="Screenshot 2026-09-09 170752" src="https://github.com/user-attachments/assets/947e670a-0ead-42ca-8139-f80a9b30d86a" />
<img width="418" height="174" alt="Screenshot 2026-09-09 170918" src="https://github.com/user-attachments/assets/d44ae3cd-cf0f-4e4c-a259-c47cdbc52672" />

---

## Overall Assessment Results

| Information Category | Result |
|----------------------|--------|
| Patient Reports | Accessed |
| Protected PDF Reports | Protection weakness identified |
| Staff Salary Information | Accessed |
| Stakeholder Information | Accessed |

---

## Key Security Concerns

The assessment identified security weaknesses primarily related to:

- **Access Control**
- **Sensitive Data Exposure**
- **Document Protection**
- **Authorization Controls**
- **Protection of Confidential Information**

These weaknesses could potentially allow an unauthorized user to access confidential patient or organizational information.

---

## Impact

Depending on the exploitation scenario, the identified weaknesses could result in:

- Unauthorized access to patient information
- Exposure of confidential organizational data
- Disclosure of employee salary information
- Exposure of stakeholder information
- Privacy and compliance risks
- Potential reputational damage

---

## Recommended Security Improvements

The following measures are recommended:

1. Implement strong role-based access controls.
2. Enforce server-side authorization checks for sensitive resources.
3. Protect sensitive documents using robust security mechanisms.
4. Avoid relying solely on client-side access restrictions.
5. Apply the principle of least privilege.
6. Conduct regular security testing of sensitive data handling.
7. Implement proper logging and monitoring for access to confidential information.
8. Retest the application after remediation.

---

## Tools & Technologies

Tools used during the assessment may include:

- Kali Linux
- Burp Suite
- Nmap
- PDF security analysis tools
- Browser Developer Tools
- Command-line utilities

---




## This repository is intended strictly for educational and authorized cybersecurity testing purposes.
