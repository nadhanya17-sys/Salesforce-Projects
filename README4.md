# Space Station Resource Management – Salesforce Capstone Project

## Project Overview

This project demonstrates how Salesforce can be used to manage a large-scale engineering initiative: building a space station for a multiplanetary civilization.
The application helps track **project status, manpower utilization, and supply costs** using Salesforce configuration, automation, reports, and dashboards.

---

# Business Problem

As the project to build a large space station begins, project managers realize that managing **resources, manpower, and supplies** manually would be inefficient.

They need a centralized system to:

* Track construction progress
* Monitor manpower utilization
* Manage supply inventory and costs
* Analyze project resource usage

The organization decides to use Salesforce to build a custom **Space Station Resource Management Application**.

---

# Data Model Design

Three custom objects were created to manage the project data.

---

## Station (Main Object)

This is the **primary object** used to track the overall project.

### Fields

* **Name** (Standard field)
* **Project Status** (Picklist: Planned, In Progress, Completed)
* **Sum of Resources** (Roll-Up Summary Field)

### Relationships

* Master-Detail relationship with:

  * Man-Power
  * Supply

This allows Salesforce to aggregate resource data at the Station level.

---

##  Man-Power Object

Tracks workforce utilization for the project.

### Fields

* **Shift** (Picklist)
* **Department** (Text)
* **Total Number of People in Department** (Number)
* **Percentage Utilization of Manpower** (Percent)
* **Total Crew** (Formula Field)

### Relationship

* Master-Detail relationship with **Station**

---

##  Supply Object

Tracks supplies required for construction.

### Fields

* **Supply Name** (Text)
* **Cost** (Currency)
* **Quantity** (Number)
* **Total Cost** (Formula: Cost × Quantity)

### Relationship

* Master-Detail relationship with **Station**

---

# User Interface Configuration

To improve usability across desktop and mobile:

### Page Layouts

* Customized layouts for Station, Man-Power, and Supply objects
* Organized related fields and sections

### Compact Layouts

* Configured key fields for quick viewing in record highlights

### Global Actions

* Quick creation of **Supply** and **Man-Power** records from anywhere in the app

### Mobile App Support

* Optimized layouts for the Salesforce mobile application

---

# Automation & Business Logic

Automation was implemented using **formulas, validation rules, and process automation**.

---

## Manpower Utilization Alert

### Business Rule

* Manpower utilization should **not exceed 80%**
* Minimum **50% utilization** should always be maintained

### Automation Logic

A process automation sends an **email alert to the System Administrator** when:

* Utilization is **greater than 80%**
* Utilization is **less than 50%**

This ensures project managers are immediately informed when manpower levels fall outside safe operating limits.

---

## Automatic Record Creation

Processes were created to automatically generate related records for:

* **Supply**
* **Man-Power**

This reduces manual data entry and improves efficiency.

---

# Reports Created

The following reports were built to analyze project performance:

1. **Supply Cost Report**

   * Tracks total cost of supplies used in construction

2. **Manpower Utilization Report**

   * Shows workforce usage by department and shift

3. **Project Status Report**

   * Displays the progress of the space station construction

---

# Dashboard

A dashboard was created to visualize key project metrics:

* Total supply cost
* Manpower utilization percentage
* Project completion status

This allows project managers to quickly monitor project health.

---

# 🛠 Salesforce Features Used

* Custom Objects
* Master-Detail Relationships
* Formula Fields
* Roll-Up Summary Fields
* Validation Rules
* Process Automation
* Page Layouts
* Compact Layouts
* Global Actions
* Reports
* Dashboards

---

# Screenshots


* Data model relationships
* Page layout configuration
* Automation process configuration
* Reports
* Dashboard

---

# Outcome

* Centralized management of project resources
* Real-time visibility into manpower and supply costs
* Automated alerts for manpower utilization
* Improved decision-making through reports and dashboards

---

# Key Learning

This project demonstrates how Salesforce can be used beyond traditional CRM to manage **large-scale operational projects through custom applications and automation**.
