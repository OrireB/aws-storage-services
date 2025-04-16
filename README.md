# AWS Storage Services

This project involves creating an AWS S3 bucket to upload, retrieve, and delete objects. It also includes configuring public access permissions and hosting HTML files from frontend mentee as a static website.

## Project Completed

1. Created an S3 bucket named `my-first-bucket-project-test`
2. Uploaded, retrieved, and deleted objects
3. Configured bucket permissions and policy to allow public access
4. Hosted a static website from a frontend mentee
5. Managed bucket and objects using AWS CLI

## Mentee Details
**Mentee Name**: Patricia Ada  
**Website Hosted**: [View Website](https://my-first-bucket-project-test.s3.us-east-1.amazonaws.com/index.html)

## Bucket Policy

{
   "Id": "Policy1",
   "Version": "2012-10-17",
   "Statement": [
       {
           "Sid": "Stmt1",
           "Action": [
              "s3:GetObject"
           ],
           "Effect": "Allow",
           "Resource": "arn:aws:s3:::my-first-bucket-project-test/*",
           "Principal": "*"
       }
   ]
}	

## Use AWS CLI to Manage S3 Buckets and Objects

- **Make sure AWS CLI is configured**:
  
  aws configure

- **List buckets**:

   aws s3 ls

- **List objects in bucket**:

  aws s3 ls s3://my-first-bucket-project-test/

- **Sync local directory to S3**:

  aws s3 sync ./local-folder/ s3://my-first-bucket-project-test/

- **Delete bucket**:

  aws s3 rb s3://my-first-bucket-project-test --force

  OR

  aws s3 rm s3://my-first-bucket-project-test/ --recursive

## Screenshots

Here are the key screenshots:

- **Screenshot 1**: S3 console showing uploaded files
  ![S3 console showing uploaded files](https://github.com/OrireB/aws-storage-services/blob/main/S3%20Uploaded%20files.png?raw=true)

- **Screenshot 2**: Bucket policy
  ![Bucket policy](https://github.com/OrireB/aws-storage-services/blob/main/Bucket%20policy.png?raw=true)

- **Screenshot 3**: The live site in the browser
  ![The live site in the browser](https://github.com/OrireB/aws-storage-services/blob/main/Live%20site%20in%20the%20browser.png?raw=true)

## Architectural Diagram

![Architecture](architecture-diagram.png)

