Salesforce Administrator

# Salesforce Security Model Implementation – Stark Corp

## Scenario
Sam, an experienced CRM leader, joined Stark Corp as a Sales Executive with a marketing background. 
He reports directly to the CEO and requires controlled access to various Salesforce objects and apps.

This project demonstrates implementation of Salesforce's multi-layer security model.

# Layer 1: Object-Level Security

## Requirement
Ensure Sam can:
- View and edit Accounts and Opportunities
- View Campaigns (marketing background)
- Not access sensitive HR custom objects
## Solution Implementation

### Profile Configuration
- Assigned "Sales Executive" profile to Sam.
- Enabled:
  - Read, Create, Edit on Accounts
  - Read, Create, Edit on Opportunities
  - Read access on Campaigns
- Removed access to restricted custom objects.

### Permission Sets
To provide additional temporary marketing privileges:
- Created "Marketing Access" Permission Set
- Granted Campaign Member edit access
- Assigned to Sam

## Key Concept Clarification

Object-level access is controlled by:
- Profiles (base access)
- Permission Sets (additional access)
- OWD (Organization-Wide Defaults) controls record-level access, not object visibility.

