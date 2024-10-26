# Step 1: Environment Setup

## Purpose
Set up the basic AWS environment, configure IAM, enable MFA, and create billing alerts.

## Steps
1. Enable MFA for the root account.
2. Set up IAM with least privilege roles.
3. Configure billing alerts to monitor spending.

## Code/Commands
- Instructions for setting up billing alerts, IAM policies, etc.

1. Enable MFA for the root account: 
- I am logged into the AWS Management Console 
- Searched for IAM on the search bar
- Then under security recommendations - I clicked on add MFA
- It will then take you to IAM > Security credentials

2. Set up IAM with least privilege roles 
- This step is to follow the principle of least priivilege 
- I go to IAM console
- Select roles from the access management section
- Create a new role with ReadOnlyAccess or Custom Roles

3. Configure billing alerts to monitor spending
- I navigate to the Billing and Cost Management Console
- Ensure that you have an IAM User and Role Access to Billing Information
- Then under billing and cost management, enable billing alerts
- Then go to Cloud Watch and create an alarm with the billing metric

