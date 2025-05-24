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
# Loan Application Management System (PHASE III)

## 📌 Problem Statement

Many financial institutions handle loan applications manually or through fragmented systems, which leads to inefficiencies and delays in processing. This project aims to model and implement an automated Loan Application Management System that streamlines customer loan requests, evaluates their eligibility, and processes approvals or rejections through structured data flow and decision-making logic.

## ✅ Objectives

- Automate the loan application process
- Ensure consistent eligibility checks and decision-making
- Track document submission and status
- Integrate disbursement tracking

## 📈 Business Process (BPMN Diagram)

The business process includes the following steps:

1. A customer submits a loan application.
2. The system performs an eligibility check (credit score, income, etc.).
3. Documents are uploaded and verified.
4. A loan officer makes a decision.
5. If approved, disbursement is scheduled.



## 📌 Problem Statement
A bank needs a Management Information System (MIS) to streamline and track loan applications from start to finish. The system should support customer applications, document uploads, eligibility checks, loan officer decisions, and disbursement processing.

## 🔄 Business Process Overview (Phase 2)
The business process involves the following steps:
- A customer submits a loan application.
- Required documents are uploaded.
- The system performs an eligibility check (based on income and credit score).
- A loan officer reviews and makes a decision.
- If approved, the loan is disbursed.

### 🧩 BPMN Diagram
Refer to the [`/screenshots/bpmn_diagram.png`](./scre![loan_application_logical_model_v2_diagram](https://github.com/user-attachments/assets/a6876ce0-b92b-4974-80ec-6987ee1f8766)
enshots/bpmn_diagram.png) for the visual flow of the loan application process.

---

## 🧱 Logical Model Design (Phase 3)

### 🗂️ Entities and Attributes
- **Customer**: `customer_id (PK)`, full_name, email, phone
- **Loan_Application**: `application_id (PK)`, `customer_id (FK)`, amount, application_date, status
- **Document**: `document_id (PK)`, `application_id (FK)`, doc_type, upload_date
- **Eligibility_Check**: `check_id (PK)`, `application_id (FK)`, credit_score, income, result
- **Loan_Decision**: `decision_id (PK)`, `application_id (FK)`, `officer_id (FK)`, decision_date, decision_status
- **Loan_Officer**: `officer_id (PK)`, name, email
- **Disbursement**: `disbursement_id (PK)`, `application_id (FK)`, amount_disbursed, disbursement_date

### 🔗 Relationships
- A **Customer** can have multiple **Loan Applications**
- Each **Loan Application** can have multiple **Documents**
- Each **Loan Application** has one **Eligibility Check**, one **Loan Decision**, and one **Disbursement**
- A **Loan Officer** makes many **Loan Decisions**

### ✅ Constraints & Normalization
- All tables are normalized up to **Third Normal Form (3NF)**.
- **Constraints Used**:
  - `NOT NULL` on essential fields like IDs and status
  - `UNIQUE` on emails
  - `CHECK` on status fields (e.g., loan status, result)
  - `DEFAULT` values where applicable (e.g., default status = 'Pending')
## 📚 Normalization

The data model is normalized to **Third Normal Form (3NF)**:

- **1NF**: All attributes are atomic (e.g., no list-type values).
- **2NF**: All non-key attributes depend on the whole primary key.
- **3NF**: No transitive dependency between non-key attributes.

---

## 💡 MIS Benefits
- Enhances data consistency and access across the organization
- Supports informed decision-making by loan officers
- Reduces manual errors and speeds up processing

## 📂 Project Structure
```plaintext
LoanApplicationMIS/
├── README.md
├── screenshots/
│   ├── loan_application_bpmn.jpg
│   └── loan_application_logical_model_v2_diagram.png
├── database/
│   └── scripts.sql
└── presentation/
    └── slides.pptx

## 🗃️ Phase IV: Pluggable Database Creation and Configuration

### 🎯 Objective
To create and configure a PL/SQL Oracle Pluggable Database for the Loan Application MIS project, ensuring proper structure, access, and monitoring using Oracle Enterprise Manager (OEM).

---

### 🔧 1. Database Creation

- **Naming Convention**:  
 `  
  Example → ` GrpE_27137_holiness_loanApplicationSystem_DB`

- **Password**:  
   `holiness`

- **User Privileges**:  
  - Grant **super admin privileges** to the user
  - Create necessary tables and schemas inside this pluggable database

#### 📜 SQL Script Example
```sql
-- Create pluggable database
CREATE PLUGGABLE DATABASE GrpE_27137_holiness_loanApplicationSystem_DB
  ADMIN USER holiness IDENTIFIED BY holiness
  ROLES = (DBA);

-- Open it
ALTER PLUGGABLE DATABASE  GrpE_27137_holiness_loanApplicationSystem_DB OPEN;

-- Save state
ALTER PLUGGABLE DATABASE  GrpE_27137_holiness_loanApplicationSystem_DB SAVE STATE;

![WhatsApp Image 2025-05-25 at 01 01 51_8d252129](https://github.com/user-attachments/assets/bd1e28b6-9b32-46a3-a544-f661069a85e3)

