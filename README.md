# AWS-account-creation-and-setup (How to setup an AWS account)
## Overview
This repository provides a step-by-step guide to creating an AWS account and setting up basic security configurations to ensure a secure and well-managed cloud environment.

## Prerequisites
- A valid email address
- A phone number
- A credit/debit card for billing verification

## Steps to Create an AWS Account

### 1. Sign Up for AWS
1. Go to the [AWS Sign-Up Page](https://aws.amazon.com/)
2. Click **Create an AWS Account**
3. Enter your email, create a password, and choose an AWS account name
4. Click **Continue**
5. Enter your contact information and select **Personal** or **Business** account
6. Provide your payment details (AWS requires a credit/debit card for verification)
7. Complete phone verification by entering the code sent to your registered number
8. Choose a **Support Plan** (Basic Support is free)
9. Click **Complete Sign-Up**

### 2. Secure Your AWS Account
#### a. Enable Multi-Factor Authentication (MFA)
1. Sign in to the AWS Management Console
2. Go to **IAM (Identity & Access Management)**
3. Click on **Users** > Select your user name
4. Navigate to **Security Credentials**
5. Enable **MFA** using an authenticator app like Google Authenticator or Authy

#### b. Create an IAM User (Avoid Using Root Account)
1. Navigate to **IAM** in AWS Console
2. Click **Users** > **Add User**
3. Enter a username (e.g., `admin-user`)
4. Select **AWS Management Console Access** and set a password
5. Assign **AdministratorAccess** policy (or a custom policy based on least privilege principle)
6. Click **Create User**

#### c. Configure Billing Alerts
1. Go to the **Billing Dashboard**
2. Navigate to **Budgets** > **Create Budget**
3. Set a monthly spending limit to monitor usage

### 3. Setup CLI Access (Optional)
1. Install the AWS CLI from [AWS CLI Documentation](https://aws.amazon.com/cli/)
2. Configure AWS CLI:
   ```sh
   aws configure
   ```
3. Enter the Access Key and Secret Key from your IAM user
4. Select a default AWS region (e.g., `us-east-1`)
5. Choose a default output format (e.g., `json`)

## Best Practices
- Always use IAM users instead of the root account
- Rotate access keys regularly
- Enable **AWS CloudTrail** for logging and monitoring
- Use **AWS Organizations** to manage multiple accounts securely

## Conclusion
Your AWS account is now set up and secure. Follow best practices to maintain security and cost efficiency. For more AWS configurations, check out the AWS documentation or this repository for updates.

