# 🌐 Static Website Hosting with Amazon S3 + CloudFront

This project demonstrates how to **host a static website** using **Amazon S3** and accelerate global delivery with **Amazon CloudFront**. It is one of the fundamental setups in AWS and forms the backbone of many modern frontend deployments.

---

## 🎯 Project Goal

- Gain hands-on experience with **S3 static hosting**
- Learn how to serve content publicly via **CloudFront CDN**
- Understand basic **security settings** (bucket policies, public access)
- Deploy a globally available static site

---

## 🧰 AWS Services Used

| Service       | Purpose                                                                 |
|---------------|-------------------------------------------------------------------------|
| Amazon S3     | Host static website content (`index.html`, images, CSS, etc.)           |
| CloudFront    | Deliver content globally with low latency and caching                   |
| IAM           | (implicitly) controls access to S3 via policies                         |
| Route 53 *(optional)* | For custom domain and DNS routing (not used in this basic setup)     |

---

## 📷 Setup Steps & Screenshots

### 1. Create an S3 Bucket  
Create a globally unique bucket and disable “Block all public access”.

![S3 Bucket Created](screenshots/01-s3-bucket-created.png)

---

### 2. Enable Static Website Hosting  
Activate the static hosting feature and specify `index.html` as the root.

![Static Hosting Enabled](screenshots/02-static-hosting-enabled.png)

---

### 3. Upload Website Files  
Upload your static files like `index.html` to the bucket.

![HTML Uploaded](screenshots/03-html-uploaded.png)

---

### 4. Configure Bucket Policy  
Apply a policy to allow public read access.

![Bucket Policy](screenshots/04-bucket-policy.png)

---

### 5. Set Up CloudFront Distribution  
Configure CloudFront to use your S3 bucket as the origin and define the root object.

![CloudFront Config](screenshots/05-cloudfront-config.png)

---

### 6. Verify CloudFront Deployment  
Check the public CloudFront domain to ensure successful delivery.

![CloudFront Verified](screenshots/06-cloudfront-verified.png)

---

## 🚀 What Can Be Built on Top of This?

Once this foundational setup is understood, it opens the door to:

- ✅ **React/Vue/Angular** frontend deployments
- 📁 Versioned documentation sites (e.g., Docusaurus)
- 📦 Hosting frontends for serverless full-stack apps
- 🌍 Low-cost portfolio or personal blog hosting
- 🔐 CloudFront signed URLs for secure content delivery
- 🌐 Domain integration via Route 53 + HTTPS via ACM (SSL/TLS)

---

## 🧠 What You Learn Here Is Fundamental For:

- Serverless architecture (e.g., S3 + Lambda + API Gateway)
- CI/CD pipelines (upload build artifacts to S3)
- Multi-region content delivery strategies
- AWS Certification (SAA, DevOps, etc.)

---

## ✅ Final Outcome

You now have a fully functional, **globally available**, low-latency static website hosted on AWS — an essential building block for modern web applications and cloud-based architecture.
