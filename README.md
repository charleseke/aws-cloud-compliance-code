# AWS Cloud Compliance Code
CloudFormation templates and Service Control Policies that enforce compliance controls without manual intervention.

Infrastructure as Code (IaC) and Service Control Policies (SCPs) ensure resources deploy securely and consistently allowing you to define your entire compliance infrastructure in code, making it repeatable, testable, and auditable.

IaC ensures compliant resource deployment and SCPs create hard boundaries that prevent policy violations even when someone tries to deploy resources outside your approved templates.

## CloudFormation Resources
Instead of checking if resources are configured correctly after they’re deployed, IaC ensures they’re deployed correctly in the first place. IaC eliminates the gap between deployment and compliance validation.
- Secure S3 bucket with public access blocked and encryption enabled
- AWS Config rule that checks for a strong IAM password policy
- AWS Config rule that checks if S3 buckets have server-side encryption enabled

## Lambda Functions 
Lambda is a compute service that can serve as your automated compliance assistant, allowing you to run generated code in response to events without requiring you to manage any servers, operating systems, or infrastructure.


## Service Control Policies
Organizational-level guardrails that set boundaries on what actions can be performed across all AWS accounts in your organization.
- Prevent Audit Log Deletion
- Prevent Insecure SSH
- Require S3 encryption 
