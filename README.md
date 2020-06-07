# Static-Website-Cloud-Formation
CloudFormation scripts to run on Amazon Web Services, to create a static webiste using S3 Bucket and CloudFront distribution.

## Requirements to run the scripts on your local machine
Here are some of the requirements, to run these scripts on your local machine:
1. Download a text editor like Microsoft Visual Studio Code. Link to download Microsoft Visual Studio Code: https://code.visualstudio.com/
2. Set up an Amazon Web Services account. Here's link to create your AWS account: https://portal.aws.amazon.com/billing/signup#/start
3. Set AWS Command Line Interface on your device. Download AWS CLI tool using the link: https://aws.amazon.com/cli/.
4. Use the following command in your command prompt or terminal of your VS Code to set-up your AWS account.
`$ aws configure`
5. Follow the steps to create Access Key and Secret Access Key in IAM, using the following link: https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html#cli-quick-configuration

## Running the scripts to create cloudformation stack
1. Open VS Studio code, and open the repository containing all the file for of scripts.
2. Run the following command to create the stack to create S3 bucket: 
```
$ ./create <stack-name> bucket.yml bucket.json
```
3. (Optional) Run the following command to update the cloudformation stack: 
```
$ ./create <stack-name> bucket.yml bucket.json
```
3. Open Cloud Formation in AWS console to check if stack was created or updated successfully.
4. Upload [index.html](https://github.com/Karansingh005/Static-Website-Cloud-Formation/blob/master/index.html) to S3 bucket.
 (Alert! Deployments.yml won't work to deploy cloudfront distribution. So, to create cloudfront distribution, use AWS management console.)
