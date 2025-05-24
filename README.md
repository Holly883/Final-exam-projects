# Final-exam-projects
Phase one
# Satellite Tracking and Monitoring System 🚀

## 📌 Project Overview

The **Satellite Tracking and Monitoring System** is a PL/SQL-based Oracle database solution developed to automate the tracking, health monitoring, and management of satellites. This project simulates real-world operations of mission control centers by handling data related to satellite location, system health, signal strength, and maintenance needs.

---

## 🎯 Objectives

- Automate real-time tracking of satellites
- Monitor satellite health parameters (battery level, signal strength, etc.)
- Generate alerts for low performance or technical issues
- Maintain historical data for analysis and reporting

---

## 🏢 Context & Usage

This system is designed for **space agencies**, **private satellite companies**, and **mission control centers** that need to manage and monitor multiple satellites simultaneously with high reliability and minimal delay.

---

## 👥 Target Users

- Satellite Operators  
- Mission Control Engineers  
- Aerospace Analysts  
- Space Tech Researchers  

---

## 🧩 Main Entities

- **SATELLITES**: Stores basic satellite information  
- **TRACKING_LOG**: Logs satellite positions in orbit  
- **HEALTH_STATUS**: Stores battery life, signal strength, and temperature  
- **MAINTENANCE_ALERTS**: Generates alerts for performance issues  
- **CONTROL_TEAM**: Information about the team responsible for monitoring  

---

## 🛠️ Technologies Used

- **Oracle Database**  
- **PL/SQL (Procedures, Functions, Triggers)**  
- SQL Developer or any Oracle-compatible tool

---

## ✅ Features

- Real-time satellite tracking logs  
- Automatic alerts for critical health conditions  
- Historical reports for satellite status  
- User-friendly queries for analytics and monitoring  
- Secure, normalized data design with referential integrity  

---

## 🚀 Benefits

- 📉 Reduces satellite downtime  
- 📡 Improves tracking accuracy  
- 🛡️ Enhances data security and reliability  
- 📊 Supports long-term data analysis and predictive maintenance  

---

## 📚 Future Improvements

- AI-based health prediction models  
- Web interface integration  
- Satellite command issuing simulation

# Loan Application Process – MIS Project (Phase II)

## 📌 Problem Statement

Loan application processes often suffer from inefficiencies due to poor coordination between departments, incomplete data, and lack of decision support. This MIS project models the loan application workflow to streamline decision-making, improve data flow, and increase transparency for both bank staff and customers.

## 🎯 Objectives

- Model the current loan approval workflow using BPMN.
- Identify system actors, interactions, and decision points.
- Demonstrate how MIS supports the process by improving decision-making and reducing manual errors.

---

## 🔄 Methodology

We used **Business Process Model and Notation (BPMN)** to model the flow of the loan application. The model was created using Lucidchart and shows interactions across:
- Customers
- Bank Front Desk
- Loan Approval Department

The diagram uses **swimlanes** to distinguish responsibilities and ensure clarity in process steps.

---

## 👥 Key Entities and Roles

| Entity              | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| **Customer**        | Submits application, provides documents, accepts/rejects loan offer         |
| **Front Desk**      | Checks customer status, collects and verifies documents                     |
| **Bank System**     | Analyzes transactions, checks financial eligibility                         |
| **Loan Department** | Decides loan approval, generates agreements, and communicates decisions     |

---

## 🖼️ BPMN Diagram

![Loan Process BPMN](./screenshots/loan_process_bpmn.jpg![WhatsApp Image 2025-05-18 at 22 12 26_e293722b](https://github.com/user-attachments/assets/f341cac7-01ec-441c-9ed5-3657267ff469)
)

---

## 🔍 Explanation of the Diagram

- **Start:** Customer submits a loan request and required documents.
- **Document Check:** Front Desk verifies if the documents are complete and checks if the customer is existing or new.
- **Eligibility Analysis:** The system evaluates financial eligibility and transaction history.
- **Loan Approval:** If eligible, the loan is approved, terms are proposed, and the customer decides to accept or reject.
- **End:** Loan is either disbursed or rejected, and the customer is notified.

This process supports **MIS functions** by:
- Improving decision-making via system-based eligibility checks.
- Reducing delays through streamlined workflows.
- Supporting data accuracy by using digital systems instead of manual decisions.

---

## 🗃️ Database Design (for upcoming phases)

[To be completed in later phases: includes ERD, normalization, and PL/SQL implementation.]

---

## 🧠 Tools Used

- **Lucidchart** for diagramming
- **Markdown** for README documentation
- **GitHub** for version control and presentation

---

## ✅ Conclusion

The BPMN model improves clarity and organizational efficiency, ensuring that all steps are well-documented and decision-making is optimized through MIS.



