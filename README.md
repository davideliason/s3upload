# s3Upload
## January 24, 2018
### [David Eliason](http://www.davethemaker.com)

### Description
This is a proof of concept low-level application that focuses on the AWS s3 funcitonality of allowing access to s3 bucket to upload a file. The AWS example brings in federated identities, using such things as Google+ or Facebook, for accessing the s3 bucket, which is great for production, but to better understand the process, this application really strips down things to a basic level.

### Steps
1. Created IAM (AWS Identity and Access Management) user with full S3 access, downloaded Access Key ID and Secret Access Key. This was a new identity separate from my root user policy.
2. Configured S3 bucket with FullAccess permissions
3. Created html document which will use vanilla JS event handlers to allow file selection and then posting new s3 object using the AWS config and file data

### Next steps:
Next steps would be to fine tune access permissions, either by creating an authorization via application login, or by going the route of federated identities as the AWS example suggests. 

![Form]('./s3UploadFileUpload.png')
![Result]('./s3UploadResult.png')
[great resource](http://adventure-us.guide/uploading-images-s3-using-javascript-aws-sdk/)