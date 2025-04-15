# AWS Storage Services

This project involves creating an AWS S3 bucket to upload, retrieve, and delete objects. It also includes configuring public access permissions and hosting HTML files from frontend mentee as a static website.

## 📌 Tasks Completed

1. Created an S3 bucket named `my-first-bucket-project-test`
2. Uploaded, retrieved, and deleted objects
3. Configured bucket permissions and policy to allow public access
4. Hosted a static website from a frontend mentee
5. Managed bucket and objects using AWS CLI

## 👨‍🎓 Mentee Details
**Mentee Name**: Patricia Ada  
**Website Hosted**: [View Website](https://my-first-bucket-project-test.s3.us-east-1.amazonaws.com/index.html)

## 📸 Screenshots

Here are the key screenshots:

- **Screenshot 1**: S3 console showing uploaded files
  ![S3 console showing uploaded files](https://github.com/OrireB/aws-storage-services/blob/main/S3%20Uploaded%20files.png?raw=true)

- **Screenshot 1**: Bucket policy
  ![Bucket policy](https://github.com/OrireB/aws-storage-services/blob/main/Bucket%20policy.png?raw=true)

- **Screenshot 1**: The live site in the browser
  ![The live site in the browser](https://github.com/OrireB/aws-storage-services/blob/main/Live%20site%20in%20the%20browser.png?raw=true)

## Bucket Policy

{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::frontend-website-host-bucket/*"
    }
  ]
}


## 📐 Architectural Diagram

![Architecture](architecture-diagram.png)

