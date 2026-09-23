# Secure Static Website using AWS S3 and CloudFront

## Project Overview

This project demonstrates how to host a static website using a
private Amazon S3 bucket and Amazon CloudFront.

The S3 bucket is not publicly accessible. CloudFront accesses the
S3 bucket using Origin Access Control (OAC).

## Architecture

Internet
|
v
CloudFront
|
| OAC
v
Private S3 Bucket

## AWS Services Used

- Amazon S3
- Amazon CloudFront
- Origin Access Control (OAC)
- IAM

## Features

- Static website hosting
- Private S3 bucket
- CloudFront distribution
- Origin Access Control
- No direct public access to S3
- HTTPS delivery through CloudFront

## Security

Block Public Access is enabled on the S3 bucket.

Only CloudFront is allowed to retrieve objects from S3.

## Project Structure

```text
.
├── index.html
├── style.css
└── README.md
```
