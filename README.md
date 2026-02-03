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

## 🔧 Setup & Usage
1. Upload your website files to an S3 bucket.
2. Enable static website hosting on the bucket.
3. Create a CloudFront distribution pointing to the S3 bucket origin.

## ✅ Verification
- Access the website using the CloudFront domain name (e.g., `dxxxxx.cloudfront.net`).

---
Created by **Tunahan Koç** | [LinkedIn](https://www.linkedin.com/in/tunahan-koc-8b43b765/) | [GitHub](https://github.com/tnhkoc)
