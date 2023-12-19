# Week 0 — Billing and Architecture

## Basic Learning
Commenced this bootcamp on December 16th, 2023. During this period, I gained insights into the following:
- AWS Well-Architected Framework
- TOGAF (basic understanding)
- c4model.com
- Received initial instructions from bootcamp instructors to document progress in the form of a journal.

## AWS Setup
1. **AWS User Account Creation:**
   - Set up an AWS User Account for improved security.
   - Enabled Multi-Factor Authentication (MFA) on the root account.
   - Created an IAM user and added it to the admin group.
   - Adopted the IAM user for future activities.
   - Generated Access Keys in security credentials.
   - Utilized AWS CLI in CloudShell for a sanity check, confirming the correct account with the command `aws sts get caller-identity`.

## Gitpod Workspace
1. **Installing AWS CLI:**
   - Opened the GitHub repo in Gitpod.
   - Installed AWS CLI in the VSCode terminal using the official documentation.
   - Configured the `.gitpod.yml` file to ensure automatic setup of configurations on workspace launch ([gitpod.yml](/.gitpod.yml)).
2. **Verification:**
   - Configured environment variables via Gitpod's account settings or using commands like 'export' or 'gb env'.

## Alarm and Billing Setup
- Implemented alarm setup using the CLI; equivalent configurations can be done through the GUI ([code files](/aws)).
- IAM admin does not have billing access by default; root has the access. Pricing varies by region with 10 free alarms in the free tier.
- Leveraged features like cost allocation tags and cost explorer.
- Utilized calculator.aws for effective cost estimation.

## Security
- Gained insights into security from a guest lecturer:
   - Explored topics like Root User, MFA Enablement, AWS CloudTrail Enablement, and various IAM user types (e.g., federated).
   - Discussed roles and implemented the AWS Well-Architected Framework.

## Diagrams in Lucid Chart
- Created conceptual ([link here](https://lucid.app/lucidchart/d46959f0-bfc0-407c-acf1-879ea9f447f5/edit?viewport_loc=-1737%2C-19%2C2125%2C1117%2C0_0&invitationId=inv_d9387379-3c36-47c1-ba78-711ef5ee28da)) and architectural ([link here](https://lucid.app/lucidchart/861468ef-681e-4c61-bb70-97a9d5b8cf72/edit?viewport_loc=392%2C-1158%2C3188%2C1676%2C0_0&invitationId=inv_26dee339-9016-4d47-9ba8-e577e9e7a61e)) diagrams.
  
  ![Conceptual Diagram](/assets/w00-conceptual-diagram.png)
  
  ![Architectural Diagram](/assets/w00-Architectural-Diagram.png)

## Learning Markdown Language
Explored the Markdown language and its application in journal writing for documentation purposes.

## Hiding Sensitive Data and Credentials
Learned about tools such as BFG Repo Cleaner and Trufflehog for removing sensitive data or credentials committed to repositories.
