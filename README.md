# 🌐 Static Website Hosting with Amazon S3 and CloudFront

This project demonstrates how to host a static website using Amazon S3 and distribute it globally using Amazon CloudFront.

---

## 🎯 Project Objectives

- Learn to configure static website hosting using Amazon S3
- Understand how CloudFront enhances website performance and delivery
- Gain experience with public access settings and content distribution

---

## 🧰 AWS Services Used

- **Amazon S3** – Static file storage and website hosting
- **Amazon CloudFront** – Global content delivery and caching service
- **IAM** – (Optional) Access control, not explicitly used in this project

---

## 🗺️ Architecture Flow

- User → CloudFront → S3 Bucket (Static Website Hosting)

---

## 🛠️ Setup Steps & Screenshots

### 1. Create an S3 Bucket  
Create a new bucket with a globally unique name and disable “Block all public access”.  
📸 `screenshots/01-s3-bucket-created.png`

---

### 2. Enable Static Website Hosting  
Enable the “Static website hosting” option and set the index document (e.g., `index.html`).  
📸 `screenshots/02-static-hosting-enabled.png`

---

### 3. Upload HTML Content  
Upload your `index.html` or any static site files to the S3 bucket.  
📸 `screenshots/03-html-uploaded.png`

---

### 4. Configure Bucket Policy  
Allow public read access by applying a bucket policy that grants access to all objects.  
📸 `screenshots/04-bucket-policy.png`

---

### 5. Set Up CloudFront Distribution  
Create a CloudFront distribution with the S3 bucket as the origin. Set the default root object to `index.html`.  
📸 `screenshots/05-cloudfront-config.png`

---

### 6. Verify Website via CloudFront URL  
After deployment, visit the CloudFront domain to access your site.  
📸 `screenshots/06-website-verified.png`

---

## ✅ Result

You’ve successfully deployed a fast, globally available static website using Amazon S3 and CloudFront.

---

## 💰 Cost Consideration

✅ **Free Tier Friendly**  
- S3: 5 GB storage, 20,000 GET, 2,000 PUT requests/month  
- CloudFront: 1 TB data out/month & 2M requests  

Monitor AWS billing to stay within limits.

---

## 📁 Project Structure

static-website-s3-cloudfront/
├── README.md
├── index.html
└── screenshots/
├── 01-s3-bucket-created.png
├── 02-static-hosting-enabled.png
├── 03-html-uploaded.png
├── 04-bucket-policy.png
├── 05-cloudfront-config.png
└── 06-website-verified.png
