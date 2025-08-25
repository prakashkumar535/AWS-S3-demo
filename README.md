# AWS S3 Setup with ASP.NET Core Web API  

This project demonstrates how to integrate **Amazon S3** into an **ASP.NET Core Web API** using the **AWS SDK for .NET**.  
It exposes REST endpoints to perform all **basic bucket and file operations** on AWS S3.  

---

## 🚀 Features  

### 📂 Bucket Operations (BucketsController)
- **Get All Buckets** → List all available S3 buckets  
- **Create Bucket** → Create a new bucket if it does not exist  
- **Delete Bucket** → Remove an existing S3 bucket  

### 📄 File/Object Operations (FilesController)
- **Upload File** → Upload a file to an S3 bucket (with optional prefix/folder)  
- **Get All Files** → List all files in a bucket with **Pre-signed URLs** for secure temporary access  
- **Get File by Key** → Download a specific file by object key  
- **Delete File** → Delete a specific file from a bucket  

---

## 🛠️ Tech Stack
- **ASP.NET Core Web API**  
- **AWS SDK for .NET (S3)**  
- **Amazon S3**  

---

## 🔑 Prerequisites
- AWS account  
- IAM user with S3 permissions:  
  - `s3:ListBucket`  
  - `s3:CreateBucket`  
  - `s3:DeleteBucket`  
  - `s3:PutObject`  
  - `s3:GetObject`  
  - `s3:DeleteObject`  
- AWS Access Key & Secret Key  
- [.NET 6/7/8 SDK](https://dotnet.microsoft.com/download) installed  

---

## 🔧 Setup & Configuration  

### 1️⃣ Install Required Packages  
Run the following commands in the **Package Manager Console**:  

```powershell
Install-Package AWSSDK.S3
Install-Package AWSSDK.Extensions.NETCore.Setup
