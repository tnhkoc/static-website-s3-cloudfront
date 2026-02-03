# Static Website Hosting (S3 + CloudFront)
> Global content delivery for static sites using Amazon's CDN.

## 🎯 Objective
Demonstrates the deployment of a high-performance static website hosted on S3 and distributed globally via Amazon CloudFront for low-latency access.

## 🚀 Key Features
- **Global Scalability:** Uses CloudFront edge locations for fast content delivery.
- **Secure Access:** Configures S3 bucket policies to allow access only via CloudFront (OAC/OAI).
- **Cost-Effective:** Serverless hosting with no management overhead.

## 🏗️ Architecture
```mermaid
flowchart LR
  User((User)) -->|HTTPS| CF["CloudFront Distribution"]
  CF -->|Fetch| S3["S3 Static Bucket"]
```

## 🛠️ Tech Stack
- **Storage:** Amazon S3
- **CDN:** Amazon CloudFront
- **Security:** OAC (Origin Access Control)

---

## 🔧 Setup & Implementation

### 1. S3 Bucket Setup
![S3 Bucket](screenshots/01-s3-bucket-created.png)
Enable static website hosting.
![Static Hosting](screenshots/02-static-hosting-enabled.png)

### 2. Content Upload
![Upload HTML](screenshots/03-html-uploaded.png)

### 3. CloudFront & Security
Configure the distribution and restrict bucket access.
![CloudFront Config](screenshots/05-cloudfront-config.png)
![Bucket Policy](screenshots/04-bucket-policy.png)

## ✅ Verification
Access the site via the CloudFront domain.
![Verified](screenshots/06-cloudfront-verified.png)

---
Created by **Tunahan Koç** | [LinkedIn](https://www.linkedin.com/in/tunahan-koc-8b43b765/) | [GitHub](https://github.com/tnhkoc)
