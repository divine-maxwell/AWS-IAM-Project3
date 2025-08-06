# 🔐 AWS IAM Project 3 – Group Policy & Least Privilege Enforcement

## 📌 Project Overview
This project demonstrates how to implement **IAM Group-based permissions** using AWS IAM.  
The goal was to validate the **Principle of Least Privilege** by attaching a read-only S3 policy to a group, adding users to it, and testing access behavior.

---

## 🛠️ What I Did
1. Created an IAM group called `Testers`.
2. Attached the managed policy `AmazonS3ReadOnlyAccess` to the group.
3. Created IAM users and added them to the group.
4. Logged in as the test users and performed:
   - ✅ Read operations on S3
   - ❌ Write operations (upload/delete) — blocked
5. Verified permission enforcement through direct AWS Console testing.

---

## ✅ Test Results

| Action Tested             | Result     | Screenshot |
|---------------------------|------------|------------|
| IAM Group Created         | ✅ Success  | [📸 View](./screenshots/iam-group-created.png) |
| Users Added to Group      | ✅ Success  | [📸 View](./screenshots/user-added-group.png) |
| Group Permissions Verified| ✅ Success  | [📸 View](./screenshots/group-permissions.png) |
| Read Access to S3         | ✅ Success  | [📸 View](./screenshots/s3-read-success.png) |
| Upload to S3 Attempt      | ❌ Denied   | [📸 View](./screenshots/s3-upload-blocked.png) |
| Policy Confirmed in User  | ✅ Verified | [📸 View](./screenshots/policy-verified.png) |

---

## 🖼️ Screenshot Previews

| Description | Preview |
|-------------|---------|
| IAM Group Creation | [<img src="./screenshots/iam-group-created.png" width="200"/>](./screenshots/iam-group-created.png) |
| User Added to Group | [<img src="./screenshots/user-added-group.png" width="200"/>](./screenshots/user-added-group.png) |
| Group Permissions | [<img src="./screenshots/group-permissions.png" width="200"/>](./screenshots/group-permissions.png) |
| Policy Verified in User | [<img src="./screenshots/policy-verified.png" width="200"/>](./screenshots/policy-verified.png) |
| S3 Read Success | [<img src="./screenshots/s3-read-success.png" width="200"/>](./screenshots/s3-read-success.png) |
| S3 Upload Blocked | [<img src="./screenshots/s3-upload-blocked.png" width="200"/>](./screenshots/s3-upload-blocked.png) |

---

## 🧰 AWS Services Used

- **IAM** – Identity and Access Management
- **S3** – Simple Storage Service (for testing access)
- **AWS Console** – Used to configure and test

---

## 🔐 Security Concepts Demonstrated

- IAM Group-based Permission Assignment
- Use of AWS Managed Policies
- Role-based Access Control (RBAC)
- Least Privilege Enforcement
- Access Validation through Simulation

---

## 📁 Project Structure

aws-iam-project3/
├── README.md
└── screenshots/
├── iam-group-created.png
├── user-added-group.png
├── group-permissions.png
├── policy-verified.png
├── s3-read-success.png
└── s3-upload-blocked.png

---

✅ **This project highlights my ability to apply IAM group policies, enforce access control, and validate permissions through testing in AWS.**
