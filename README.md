# AWS S3 Access Using EC2 Instance Profile

## Project Overview
This project demonstrates secure access to an Amazon S3 bucket from an EC2 instance using an IAM Role (Instance Profile) without storing AWS access keys on the server.

## Services Used
- Amazon EC2
- Amazon S3
- AWS IAM
- AWS CLI

## Architecture
EC2 Instance → IAM Role → S3 Bucket

## Steps Performed
1. Created an S3 bucket.
2. Uploaded files to the bucket.
3. Created an IAM Role with S3 permissions.
4. Attached the IAM Role to the EC2 instance.
5. Connected to the EC2 instance using SSH.
6. Verified access using AWS CLI.

## Commands Used

```bash
aws sts get-caller-identity
aws s3 ls
aws s3 ls s3://bucket-name
aws s3 cp file.txt s3://bucket-name/
