# AWS CodeBuild Hands-on 

## Overview
Created a simple AWS CodeBuild project using Amazon S3 as the source.

## Architecture

VS Code
↓
ZIP Project
↓
S3 Source Bucket
↓
AWS CodeBuild
↓
Build Artifact
↓
S3 Artifact Bucket

## AWS Services Used
- Amazon S3 – Stores source ZIP and build artifact
- AWS CodeBuild – Builds the application
- IAM – Provides permissions to CodeBuild

## Project Files

codebuild-demo/
├── index.html
└── buildspec.yml

## Steps
1. Created `index.html` and `buildspec.yml`.
2. Created a ZIP file containing both files.
3. Uploaded the ZIP to an S3 source bucket.
4. Created an AWS CodeBuild project.
5. Configured Amazon S3 as the source provider.
6. Configured `buildspec.yml` for build commands.
7. Configured an S3 bucket for build artifacts.
8. Started the build and verified **BUILD SUCCEEDED**.
9. Verified the generated `codebuild-output.zip` in the artifact bucket.

## Result
The CodeBuild project successfully built the application
and stored the build artifact in Amazon S3.

## Key Learning
AWS CodeBuild automates the build process by taking source code,
executing commands defined in `buildspec.yml`, and generating a build artifact.

## CREATED BY 
JAWERIYA MAHIN
