# cloudresumeproject

www.emiroz.com

In this project I created a website to host my resume. The website contact form is connected to a Database and Notification Service to store each and notify me when there is a submission. Services that I used: AWS S3, SNS, DynamoDB, Route 53, ACM, CloudFront, IAM, Lambda and API Gateway. The following steps were taken in order to complete this project:

	Created a S3 Bucket and enable the static website hosting.
	Created a SNS topic and created subscription with email protocol.
	Created DynamoDB table with partition key and sort key.
	Registered a new domain with using Route 53 then requested a public certificate for my domain by using Amazon Certificate Manager.
	Created CloudFront distribution for my root object which stored in my S3 bucket.
	Created simple routing policy record set for my domain with using Route 53.
	Created Lambda function to run the scripts. I granted full access of DynamoDB and SNS to the new role that I got with creating this lambda function.
	Finally created a REST API to trigger with using Amazon API Gateway and copied invoke url to my html code.
