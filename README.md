# -Secure-Multi-Tier-Access-Management-System-Using-AWS-IAM
To design and implement a secure and scalable IAM strategy for a simulated enterprise application hosted on AWS, demonstrating how to manage Users, Groups, Policies, and Roles effectively with least-privilege access.

# 🚀 AWS IAM Access Management using CloudFormation

This project defines a secure and scalable AWS Identity and Access Management (IAM) structure using **AWS CloudFormation**, enabling centralized control over user access, roles, policies, and resource permissions in an enterprise-grade AWS environment.

---

Project Architecture:
Departments (Groups):

Developers

DevOps

Security

Managers

Users:

Create 2 users for each department (total: 8 users).

Assign users to appropriate groups.

Policies (JSON based):

Custom policies tailored for each group.

Example:

Developers: Read/write access to S3, access to CodeCommit.

DevOps: Full access to EC2, CloudWatch, limited IAM access.

Security: Read-only access to CloudTrail, IAM, and S3.

Managers: Billing and cost explorer access, read-only to other services.

Roles:

Cross-account role: Simulate a role that allows read-only access from another AWS account.

EC2 Role: Attach to an EC2 instance to allow access to S3 buckets without using access keys.

