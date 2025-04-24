# 🛡️ Transaction Web App Threat Model

This project is a **simulated threat model** of a basic web application inspired by M-Pesa. It is built using the [Microsoft Threat Modeling Tool (TMT)](https://aka.ms/tmt).

> This hands-on project applies the STRIDE methodology to analyze a mobile payment system architecture.

---

## 🧩 Components Modeled

- **Web Client** — Login & initiate transactions
- **Web Server** — Business logic and API gateway
- **Authentication Server** — Identity & session management
- **Database** — Secure storage for users and transactions
- **External M-Pesa API** — Simulated mobile money interface

---

## 🔐 STRIDE Threat Analysis Summary

| STRIDE Category            | Example Threats Identified                      |
|----------------------------|-------------------------------------------------|
| **Spoofing**               | Identity spoofing via weak login                |
| **Tampering**              | Modified transaction requests                   |
| **Repudiation**            | Denial of actions without logs                  |
| **Information Disclosure** | Sensitive data in clear text transmission       |
| **Denial of Service**      | Overload on API endpoints, HTTPS interruption   |
| **Elevation of Privilege** | Bypassing role-based controls, impersonation    |

---

## 📊 Threats at a Glance

| ID | Title                                               | Category               | Priority | State        |
|----|-----------------------------------------------------|------------------------|----------|--------------|
| 1           | Potential Data Repudiation by Service App              | Repudiation            | High          | Not Started  |
| 2           | Potential Process Crash or Stop for Service App     | Denial Of Service      | High          | Not Started  |
| 3           | Data Flow HTTPS Is Potentially Interrupted          | Denial Of Service      | High          | Not Started  |
| 4           | Elevation Using Impersonation                       | Elevation Of Privilege | High          | Not Started  |
| 5           | Remote Execution via Elevated Privilege             | Elevation Of Privilege | High          | Not Started  |

> View the full dataset in `Report.csv` for a complete breakdown of threats, interactions, and descriptions.

---

## 📂 Files Included

- `Report1.htm` — Full export from Microsoft TMT  
- `Service application threat model sample.tm7` — The editable threat model file  
- `diagram.png` — Visual system diagram  
- `Report.csv` — Raw threat listing exported for further analysis


## 👤 Author

**c0mmand3r**  
🔗 Connect with me: [LinkedIn](#) | [Medium](#) | [Twitter](#)

---

⚠️ **Disclaimer:** This is a hypothetical threat model created for learning and educational purposes only. For production applications, always adopt a security-by-design approach with real threat assessments.
