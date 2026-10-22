# AWS Static Website Hosting using Terraform

##  Project Overview

This project demonstrates static website hosting on AWS using Terraform.

The infrastructure includes Amazon S3, Amazon CloudFront, Amazon Route 53, and AWS Certificate Manager (ACM). Terraform modules are used to manage AWS resources.

The website is accessible through a custom domain with HTTPS enabled.

##  Architecture Diagram

<img width="1536" height="1024" alt="Architecture" src="https://github.com/user-attachments/assets/3111500b-6365-4fb8-ac79-6bf108c3cf33" />


##  Architecture Flow

1. **User** – Accesses the website using the custom domain.
2. **Amazon Route 53** – Routes the domain to the CloudFront distribution.
3. **Amazon CloudFront** – Delivers website content to users.
4. **Amazon S3** – Stores the static website files.
5. **AWS Certificate Manager (ACM)** – Provides the SSL/TLS certificate for HTTPS.
6. **Terraform** – Provisions and manages AWS infrastructure using modules.

##  AWS Services Used

* Amazon S3
* Amazon CloudFront
* Amazon Route 53
* AWS Certificate Manager (ACM)
* Terraform

##  Project Configuration

* **Project Name:** `static-web-hosting-using-terraform`
* **AWS Region:** `ap-south-1` (Mumbai)
* **S3 Bucket:** `dev-pooja-123`
* **Custom Domain:** `dev.poojadaingade.shop`
* **Hosted Zone:** `poojadaingade.shop`
* **CloudFront Distribution:** `static-web-hosting`
* **S3 Bucket Versioning:** Enabled
* **S3 Bucket ACL:** Private

##  Implementation Steps

1. Created an Amazon S3 bucket to store static website files.
2. Enabled S3 bucket versioning.
3. Configured the S3 bucket for private access.
4. Uploaded website files, including HTML, CSS, JavaScript, and images.
5. Configured Amazon CloudFront for content delivery.
6. Configured an ACM certificate for HTTPS.
7. Configured Amazon Route 53 to connect the custom domain to CloudFront.
8. Used Terraform modules, variables, and outputs to manage the infrastructure.
9. Verified website accessibility through the custom domain using HTTPS.

##  Security and HTTPS

* Configured the S3 bucket for private access.
* Used CloudFront to deliver website content.
* Configured HTTPS using an ACM SSL/TLS certificate.
* Connected the custom domain using Route 53.

**Note:** The ACM certificate used with CloudFront must be in the `us-east-1` region.

##  Project Verification

* Verified that website files were uploaded to S3.
* Configured the custom domain using Route 53.
* Accessed the website through `https://dev.poojadaingade.shop`.
* Verified that the website content loaded successfully in the browser.

##  Key Learnings

* Managing AWS infrastructure using Terraform.
* Working with Terraform modules, variables, and outputs.
* Hosting static website files in Amazon S3.
* Configuring CloudFront for content delivery.
* Connecting a custom domain using Route 53.
* Configuring HTTPS using AWS Certificate Manager.

##  Technologies Used

* Terraform
* Amazon S3
* Amazon CloudFront
* Amazon Route 53
* AWS Certificate Manager (ACM)

##  Author

**Pooja Daingade**

⭐ This project is part of my AWS and Terraform learning journey.
