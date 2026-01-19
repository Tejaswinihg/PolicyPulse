# PolicyPulse – Enterprise Policy Compliance & Approval System

PolicyPulse is an enterprise-style internal application used to manage company policies, multi-level approvals, and compliance tracking.  
It is designed to simulate real-world corporate workflows used in IT, HR, Finance, and Legal departments.

This project demonstrates backend-heavy business logic with role-based access, approvals, auditability, and a clean frontend for workflow validation.

---

**Key Features**

###  Authentication & Security
- JWT-based authentication
- Role-based access control (RBAC)
- Secure password handling using BCrypt
- Stateless session management

###  Policy Management
- Create company policies
- Policy lifecycle:
  - `DRAFT → IN_REVIEW → APPROVED`
  - Rejected policies return to `DRAFT`
- Policy versioning support

###  Approval Workflow
- Dedicated approver role
- Approve or reject policies with comments
- Full approval history tracking

###  Role-Based Access (Real World Mapping)

| Role           |  Capabilities 
| Admin          |  View all policies, view approval history 
| Policy Owner   | Create policy, submit for review, view approvals 
| Approver       | Approve / Reject policies, view approval history 
| Employee       | View approved policies 

---

##  Tech Stack

### Backend
- Java 17
- Spring Boot
- Spring Security
- JWT
- JPA / Hibernate
- MySQL
- Maven

### Frontend
- React (Vite)
- Axios
- React Router
- Context API
- Modern CSS layout

