# Terraform AWS S3 Bucket Project

## Project Overview

This project demonstrates how to create an AWS S3 bucket using Terraform.

Terraform is an Infrastructure as Code (IaC) tool that allows us to create and manage cloud resources using code instead of manually creating them in the AWS Console.

In this project, an S3 bucket was created and managed using Terraform.

---

## Technologies Used

* Terraform
* AWS S3
* AWS CLI
* Git
* GitHub

---

## Prerequisites

Before starting this project, make sure the following tools are installed:

* Terraform
* AWS CLI
* Git
* AWS Account

---

## Step 1: Configure AWS CLI

Configure AWS credentials using:

```bash
aws configure
```

Enter:

* AWS Access Key ID
* AWS Secret Access Key
* AWS Region

Verify AWS configuration:

```bash
aws sts get-caller-identity
```

---

## Step 2: Create Project Directory

Create a new project folder:

```bash
mkdir terraform-project2
cd terraform-project2
```

---

## Step 3: Create Terraform Configuration File

Create a file named `main.tf`.

```bash
nano main.tf
```

Add the Terraform code for creating an S3 bucket.

---

## Step 4: Initialize Terraform

Initialize the project:

```bash
terraform init
```

This command downloads the AWS provider and prepares the project.

---

## Step 5: Validate Configuration

Validate the Terraform configuration:

```bash
terraform validate
```

---

## Step 6: Preview Changes

Generate the execution plan:

```bash
terraform plan
```

Terraform shows what resources will be created.

---

## Step 7: Create the S3 Bucket

Apply the configuration:

```bash
terraform apply
```

Type:

```text
yes
```

Terraform creates the S3 bucket in AWS.

---

## Step 8: Verify Bucket Creation

Verify the bucket using AWS CLI:

```bash
aws s3 ls
```

Or check the bucket in the AWS S3 Console.

Bucket Created:

```text
om0126-terraform-demo-bucket
```

Region:

```text
us-east-1
```

---

## Step 9: Version Control Using Git

Initialize Git:

```bash
git init
```

Create `.gitignore`:

```text
.terraform/
*.tfstate
*.tfstate.*
*.pem
```

Add files:

```bash
git add .
```

Commit changes:

```bash
git commit -m "Add Terraform S3 bucket project"
```

Push to GitHub:

```bash
git branch -M main
git remote add origin <repository-url>
git push -u origin main
```

---

## Project Structure

```text
terraform-project2/
│
├── main.tf
├── .gitignore
├── .terraform.lock.hcl
└── README.md
```

---

## Commands Used

```bash
terraform init
terraform validate
terraform plan
terraform apply
terraform destroy
```

---

## Learning Outcome

Through this project, I learned:

* How to configure AWS CLI
* How Terraform works
* How to create AWS resources using code
* How to manage infrastructure with Terraform
* How to use Git and GitHub for version control

---

## Author

OM0126

B.Tech Student | Learning DevOps & Cloud Computing
