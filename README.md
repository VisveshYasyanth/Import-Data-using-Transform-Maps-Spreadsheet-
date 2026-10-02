# IMPORT DATA USING TRANSFORM MAPS (SPREADSHEET)

## 📌 Project Overview

**Import Data Using Transform Maps (Spreadsheet)** is a ServiceNow-based project developed to simplify the process of importing, managing, validating, and analysing employee information from spreadsheet data.

In many organizations, employee information is maintained in spreadsheets. Manually entering this information into ServiceNow can be time-consuming and may result in incorrect data, duplicate records, or inconsistent information.

This project provides a structured approach to importing employee data using **ServiceNow Import Sets and Transform Maps**. The spreadsheet data is first loaded into an **Employee Import / Staging Table** and then transformed into the **Employee Test Table** using predefined field mappings.

The **Employee ID** is configured as a **Coalesce Field**, allowing ServiceNow to identify existing employee records during subsequent imports. This helps reduce unnecessary duplicate records and makes repeated data imports easier to manage.

The imported employee information is also used to generate reports and an **Employee Analytics Dashboard**, providing a centralized view of employee information based on department and location.

Access to employee information is controlled using **ServiceNow Roles and ACLs**.

## 🎯 Objectives

- Import employee data from spreadsheets into ServiceNow.
- Reduce repetitive manual data entry.
- Maintain structured and consistent employee information.
- Map spreadsheet fields to appropriate ServiceNow fields.
- Use Employee ID to identify existing employee records.
- Prevent unnecessary duplicate records during re-import.
- Validate imported employee information.
- Generate reports based on department and location.
- Provide an Employee Analytics Dashboard for data visualization.
- Implement controlled access to employee information.
- Improve the overall efficiency of employee data management.

## 🛠️ Technologies Used

| Technology / Feature | Purpose |
|---|---|
| **ServiceNow** | Main development platform |
| **Import Sets** | Import spreadsheet data into ServiceNow |
| **Transform Maps** | Transform and map source data to target fields |
| **ServiceNow Tables** | Store employee information |
| **Coalesce** | Identify existing employee records |
| **ServiceNow Reports** | Generate employee-related reports |
| **ServiceNow Dashboards** | Visualize employee information |
| **Roles** | Control user permissions |
| **ACLs** | Restrict read and write access |

## 🔄 Project Workflow

```text
Spreadsheet
     ↓
Import Set
     ↓
Employee Import / Staging Table
     ↓
Transform Map
     ↓
Employee Test Table
     ↓
Reports
     ↓
Employee Analytics Dashboard
```

### Workflow Description

1. Employee information is maintained in a spreadsheet.
2. The spreadsheet is imported into ServiceNow using an **Import Set**.
3. The imported data is stored temporarily in the **Employee Import / Staging Table**.
4. The **Sample Spreadsheet Import Transform Map** maps source fields to the appropriate target fields.
5. **Employee ID** is configured as the Coalesce field.
6. Existing records are identified during subsequent imports.
7. The transformed data is stored in the **Employee Test Table**.
8. The employee information is validated.
9. Reports are generated using the imported employee data.
10. The reports are displayed through the **Employee Analytics Dashboard**.
11. Roles and ACLs control access to employee information.

## 📊 Employee Data

The spreadsheet contains employee information such as:

- Employee Name
- Email
- Department
- Employee ID
- Location

## 🗺️ Transform Map Field Mapping

| Source Field | Target Field |
|---|---|
| `u_name` | `u_employee_name` |
| `u_email` | `u_email` |
| `u_department` | `u_department` |
| `u_employee_id` | `u_employee_id` |
| `u_location` | `u_location` |

### Coalesce Field

The **Employee ID (`u_employee_id`)** is configured as the **Coalesce Field**.

This allows ServiceNow to:

- Identify existing employee records.
- Update matching records during re-import.
- Reduce unnecessary duplicate records.
- Make repeated imports easier to manage.

## ⭐ Key Features

- 📄 Spreadsheet-based employee data import
- 🔄 Automated field mapping using Transform Maps
- 🆔 Employee ID-based record matching
- 🚫 Duplicate prevention using Coalesce
- 🗃️ Centralized employee information
- 📋 Employee List Report
- 📍 Employees by Location Report
- 🏢 Employees by Department Report
- 📊 Employee Analytics Dashboard
- 🔐 Role-based access control
- 🛡️ ACL-based read and write restrictions
- ✅ Structured data validation and testing

## 📈 Reporting and Dashboard

The project includes multiple reports to make employee information easier to understand and analyse.

### 1. Employee List

Provides a detailed view of the employee records stored in the Employee Test Table.

### 2. Employees by Location

Provides a summarized view of employees based on their location.

### 3. Employees by Department

Provides a summarized view of employees based on their department.

### 4. Employee Analytics Dashboard

The reports are combined into an **Employee Analytics Dashboard**, providing authorized users with a centralized view of the employee dataset.

## 🔐 Security

Employee information is protected using ServiceNow's built-in security mechanisms.

### Roles

Roles are used to control which users can access employee information.

### Access Control Lists (ACLs)

ACLs are used to control:

- Read access
- Write access
- Modification of employee records

This ensures that only users with the appropriate permissions can view or modify employee information.

## 🧪 Testing and Results

The project was tested for the following functionalities:

- Spreadsheet import
- Import Set execution
- Field mapping
- Transform Map execution
- Coalesce functionality
- Duplicate prevention
- Re-import handling
- Employee data validation
- Reports
- Dashboard functionality
- Security and access control

### UAT Results

A total of **8 User Acceptance Testing (UAT) test cases** were completed successfully.

During testing, the following issues were identified and resolved:

- Duplicate employee records
- Blank Employee Name values
- Incorrect Location chart type

After resolving the identified issues, the final dataset contains:

> **17 Employee Records**

The completed solution demonstrates an end-to-end ServiceNow workflow for importing spreadsheet data, transforming it into structured employee records, securing the information, and presenting it through reports and dashboards.

## 🚀 Future Enhancements

The project can be further enhanced with:

- ⏰ Scheduled automatic imports
- ✅ Advanced spreadsheet validation
- 👤 Additional employee and training fields
- 📊 More interactive dashboard filters
- 🔔 Automated notifications
- 📝 Detailed import audit reports
- 🔄 Improved automated data validation
- 📈 Additional employee analytics

## 👥 Team Members

### Team ID
**SWTID-2026-8263**

### Team

1. **Raphael Rodricks S J**
2. **Visvesh Yasyanth T V**
3. **Manikandan K**
4. **Abirami S**
5. **Regana Barveen M**

## 📌 Project Summary

This project demonstrates how **ServiceNow Import Sets and Transform Maps** can be used to efficiently import employee information from spreadsheets into a structured ServiceNow table.

By using **Employee ID as a Coalesce field**, the project supports record matching and reduces unnecessary duplicates during repeated imports. Reports and an Employee Analytics Dashboard provide useful views of the employee data, while **Roles and ACLs** help protect the information.

Overall, the project provides a structured, secure, and efficient solution for **spreadsheet-based employee data management in ServiceNow**.
