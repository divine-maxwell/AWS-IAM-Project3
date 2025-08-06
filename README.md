# 🔐 IAM Project 3 – EC2 AssumeRole with S3 ReadOnlyAccess

This project demonstrates how to securely grant an EC2 instance read-only access to an S3 bucket using IAM roles and policies, following the principle of least privilege. The process includes creating the IAM role, assigning the correct trust relationship, attaching the role to the EC2 instance, and testing access behavior using AWS CLI.

---

## 📌 Project Goals

- 🔸 Create an IAM role with `AmazonS3ReadOnlyAccess`
- 🔸 Attach the role to an EC2 instance
- 🔸 Use the EC2 instance to list and read S3 objects
- 🔸 Verify that write/delete actions are denied
- 🔸 Enforce least privilege access across services

---

## 🧠 Concepts Practiced

- IAM Role and Trust Relationship configuration  
- Role-based EC2 permissions  
- S3 access control via managed policies  
- Testing permissions using the AWS Console and CLI  
- AWS resource segregation and security enforcement  

---

## 🛠️ Technologies Used

- **AWS IAM**
- **Amazon EC2**
- **Amazon S3**
- **AWS CLI**
- **AWS Management Console**
- **MacBook Terminal (zsh)**

---

## 🧪 Skills Demonstrated

- Identity-based access control  
- IAM role creation and permission boundaries  
- EC2 instance setup and role association  
- S3 bucket permission testing  
- Screenshot documentation and GitHub project structuring  

---

## 📸 Screenshot Walkthrough

| Step | Description | Preview |
|------|-------------|---------|
| 1 | EC2 Instance Launched | [<img src="screenshots/ec2-instance.1.png" width="200"/>](screenshots/ec2-instance.1.png) |
| 2 | EC2 Instance Configuration Details | [<img src="screenshots/ec2-instance.2.png" width="200"/>](screenshots/ec2-instance.2.png) |
| 3 | Launch Confirmation | [<img src="screenshots/ec2-instance.3.png" width="200"/>](screenshots/ec2-instance.3.png) |
| 4 | EC2 Dashboard Showing Running Instance | [<img src="screenshots/ec2-instance.4.png" width="200"/>](screenshots/ec2-instance.4.png) |
| 5 | IAM Role List View | [<img src="screenshots/iam-role.1.png" width="200"/>](screenshots/iam-role.1.png) |
| 6 | IAM Role Summary (AmazonS3ReadOnlyAccess attached) | [<img src="screenshots/iam-role.2.png" width="200"/>](screenshots/iam-role.2.png) |
| 7 | IAM Trust Policy Configuration | [<img src="screenshots/iam-role.3.png" width="200"/>](screenshots/iam-role.3.png) |
| 8 | EC2 Role Attachment Verified | [<img src="screenshots/iam-role.4.png" width="200"/>](screenshots/iam-role.4.png) |
| 9 | S3 Bucket Content Visible via EC2 | [<img src="screenshots/s3-upload.1.png" width="200"/>](screenshots/s3-upload.1.png) |

---

## ✅ Result

The EC2 instance successfully assumed the IAM role and was able to:

- ☑️ **Read** files from the S3 bucket  
- ❌ **Denied** upload or delete operations (as expected)

This validated that **AmazonS3ReadOnlyAccess** was enforced properly using IAM best practices.

---

## 💼 Portfolio Value

This project demonstrates practical experience with:

- Real-world IAM architecture  
- Security-first cloud operations  
- EC2-to-S3 least privilege enforcement  
- Documentation using GitHub and Markdown  

---

