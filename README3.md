# Case Creation Automation – Salesforce Capstone Project

## Project Overview
This project demonstrates how to automate Case creation using a Screen Flow in Salesforce.  
The flow allows users to submit queries related to courses and automatically create a Case record in the system.

---

## Business Requirement
The organization provides multiple training courses to students.  
Students often raise queries related to courses, instructors, or subject materials.

The company requires a structured system where users can submit their queries and automatically create a Case record for the support team to track and resolve issues.

---

## Solution Design

A **Screen Flow** was implemented to collect user information and create a Case record in Salesforce.

### Step 1 – User Input Screen
The flow prompts the user to enter the following details:

- Name
- Phone
- Email
- Course Enrolled
- Subject
- Instructor Name
- Query Description

### Step 2 – Data Validation
Input fields are validated to ensure required information is provided.

### Step 3 – Case Record Creation
The flow uses the **Create Records** element to create a Case record with the submitted details.

### Step 4 – Confirmation Message
After successful submission, the user receives a confirmation message that the Case has been created.

---

##  Salesforce Features Used
- Screen Flow
- Create Records Element
- Variables
- Flow Builder
- Case Object

---

##  Flow Components
- Screen Element – Collect user input
- Assignment Element – Store input values
- Create Records – Create Case record
- Confirmation Screen – Display success message

---

##  Screenshots
(Add screenshots of the following)

- Flow structure
- Screen input fields
- Create Records configuration
- Case record created in Salesforce

---

##  Outcome
- Automated case creation process
- Reduced manual data entry
- Improved tracking of student queries
- Faster support response time

---

##  Key Learning
- Designing user-friendly Screen Flows
- Automating case management using Flow Builder
- Implementing business requirements in Salesforce

