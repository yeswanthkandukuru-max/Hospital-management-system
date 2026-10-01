 🏥 Salesforce Hospital Management System

## Project Overview

The **Hospital Management System** is a Salesforce-based application designed to manage hospital operations such as
**patients, doctors, appointments, treatments, billing, and reception activities**.

This project is developed using **Salesforce Administrator features** such as Custom Objects, Custom Fields,
Relationships, Validation Rules, Page Layouts, Record Types, Flows, Reports, Permission Sets, Actions, and Email Templates.

---

## Project Objective

The main objective of this project is to create a centralized hospital management system in Salesforce that helps hospital staff:

* Manage patient information
* Manage doctor information
* Schedule and track appointments
* Record patient treatments
* Manage hospital bills
* Automate hospital processes
* Generate useful reports
* Send email notifications

---

## 🛠️ Salesforce Features Used

* Salesforce Lightning Experience
* Custom Objects
* Custom Fields
* Object Manager
* Lookup Relationships
* Page Layouts
* Record Types
* Validation Rules
* Global Value Sets
* Picklists
* Formula Fields
* Reports
* Custom Report Types
* Users
* Profiles
* Permission Sets
* Global Actions
* Email Templates
* Email Alerts
* Feed Tracking
  

# Project Structure

The application contains the following main custom objects:

### 1. 👤 Patient

Stores patient-related information.

Example fields:

* Patient Name
* Patient ID
* Phone
* Email
* Date of Birth
* Gender
* Address
* Blood Group

### 2. 👨‍⚕️ Doctor

Stores doctor information.

Example fields:

* Doctor Name
* Doctor ID
* Specialization
* Phone
* Email
* Department
* Availability

### 3. 📅 Appointment

Used to manage appointments between patients and doctors.

**Example fields:**

* Appointment Number
* Patient
* Doctor
* Appointment Date
* Appointment Time
* Appointment Status
* Reason for Visit

**Relationships:**

```text
Patient
   │
   └──── Appointment ──── Doctor
```

### 4. 💊 Treatment

Stores information about treatment provided to patients.

**Example fields:**

* Treatment Name
* Patient
* Doctor
* Treatment Date
* Treatment Details
* Prescription

### 5. 💰 Bills

Used to manage patient billing information.

**Example fields:**

* Bill Number
* Patient
* Treatment
* Bill Date
* Amount
* Payment Status
* Payment Method
* Due Date

# 🔗 Object Relationships

The major relationships in the project are:

```text
Patient
   │
   ├──────── Appointment ──────── Doctor
   │
   ├──────── Treatment ────────── Doctor
   │
   └──────── Bills ────────────── Treatment
```

These relationships allow hospital staff to access related information from different records.

# ✅ Validation Rules



Validation rules are configured on the **Appointment** object to prevent incorrect billing data.

Validation rules help ensure that:

* Appointment Cannot be in the Past


Validation rules are configured on the **Bills** object to prevent incorrect billing data.

Validation rules help ensure that:

* Paid Amount Cannot Be Greater Than Total Amount


# 🎨 Page Layouts & Record Types

Page layouts are configured to control:

* I created a Record type in Patient Object

  * Inpatient
  * Outpatient

# 📊 Reports

Reports are created to analyze hospital data.

Examples:

### Appointment Report

Shows:

* Patient
* Doctor
* Appointment Date
* Appointment Status

### Billing Report

Shows:

* Patient
* Bill Number
* Bill Amount
* Payment Status

### Treatment Report

Shows:

* Patient
* Doctor
* Treatment
* Treatment Date

Reports help hospital staff monitor daily activities.

# 📨 Email Templates

Email Templates are used for standard hospital communication.

Dear Patient,

We are pleased to confirm your appointment at VisionsDream Hospital.

Appointment Details:
Patient Name: 
Doctor: 
Appointment Date: 
Appointment Time: 
Reason for Visit:
Please arrive at the hospital 10–15 minutes before your scheduled appointment
Thank you for choosing VisionDream Hospital.

Regards,
VisionDream Hospital
Reception Team

# ⚡ Actions

## Global Actions

Global Actions are used to create records or perform common tasks from different areas of Salesforce.

* Create Patient
* Create Appointment

## Object-Specific Actions

Object-Specific Actions are created for individual objects.

* Create Appointment from Patient
* Create Bill from Treatment
* Create Treatment from Patient

# 🔄 Hospital Process Flow

The basic hospital process is:

```text
Patient Registration
        ↓
Appointment Creation
        ↓
Doctor Consultation
        ↓
Treatment
        ↓
Bill Generation
        ↓
Payment
        ↓
Receipt
```

---

# 🧾 Billing & Receipt Process

The billing process can be managed through the **Bills** object.

```text
Treatment Completed
        ↓
Create Bill
        ↓
Enter Bill Amount
        ↓
Select Payment Status
        ↓
Record Payment
        ↓
Generate Receipt Number
        ↓
Payment Completed
```

# 📁 Project Modules

| Module                 | Salesforce Component          |
| ---------------------- | ----------------------------- |
| Patient Management     | Patient Custom Object         |
| Doctor Management      | Doctor Custom Object          |
| Appointment Management | Appointment Custom Object     |
| Treatment Management   | Treatment Custom Object       |
| Billing Management     | Bills Custom Object           |
| Security               | Profiles & Permission Sets    |
| Validation             | Validation Rules              |
| Reporting              | Reports & Custom Report Types |
| Communication          | Email Templates               |
| User Interaction       | Actions                       |
| UI Configuration       | Page Layouts & Record Types   |
| Reports.               | Reports.                      |
| Dash Boards            | Dashboards                    |


# 📚 What I Learned

Through this project, I gained practical knowledge of:

* Salesforce CRM
* Salesforce Administration
* Custom Objects
* Custom Fields
* Object Relationships
* Lookup Relationships
* Page Layouts
* Record Types
* Validation Rules
* Reports
* Custom Report Types
* Users and Permission Sets
* Actions
* Email Templates
* Salesforce security
* Real-world Salesforce project implementation


# 👨‍💻 Project Role

**Role:** Salesforce Administrator / Associate Software Engineer

**Project:** Hospital Management System

**Platform:** Salesforce

**Environment:** Salesforce Trailhead / Developer Org

# 🏁 Conclusion

The **Salesforce Hospital Management System** demonstrates how Salesforce Administrator 
features can be used to build a real-world hospital application.

The project covers the complete basic workflow from:

**Patient Registration → Appointment → Treatment → Billing → Payment → Receipt**

It also demonstrates **security, automation, reporting, actions, and email communication** within Salesforce.
