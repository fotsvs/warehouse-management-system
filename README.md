# warehouse-management-system

# Warehouse Management System & Security Assessment

Custom web-based inventory management system developed for operational use, featuring a modern HTML frontend and Google Firestore backend.

## Security Audit & Vulnerability Assessment (AppSec)
As part of hardening this application, a client-side security assessment was conducted focusing on input validation and injection vectors:
* **Attack Scenario:** Tested for Stored HTML/Script Injection (XSS) via data input fields (e.g., worker observation notes sent from mobile/tablet interfaces to the administrative dashboard).
* **Mitigation & Findings:** Analyzed DOM rendering behavior. Confirmed that modern browser security mechanisms (HTML5 sandboxing on dynamic content rendering) successfully mitigate direct script execution, ensuring system integrity.
* **Remediation Best Practice:** Emphasized strict data handling principles (such as utilizing `textContent` over vulnerable assignment vectors) to prevent DOM-based vulnerabilities.

## Tech Stack
* Frontend: HTML5, CSS3, JavaScript (Vanilla)
* Backend / Database: Google Firebase Firestore & Authentication
