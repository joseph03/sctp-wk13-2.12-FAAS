# sctp-wk13-2.12-FAAS
Given a Lambda function that is triggered upon the creation of files in an S3 bucket, answer the following:
1.	What is the purpose of the execution role on the Lambda function?

The purpose of the execution role is to allow the writing of log file record whenever the trigger (event) created is triggered.

2.	What is the purpose of the resource-based policy on the Lambda function?

The resource-based policy is to defined what activity is going to trigger the trigger (event)

3.	If the function is needed to upload a file into an S3 bucket, describe (i.e no need for the actual policies)
-	What is the needed update on the execution role?

No change is needed to be made on execution role as the role has already had right to write record to log file

-	What is the new resource-based policy that needs to be added (if any)?

The resource-based policy needs to be added is the policy to trigger the selected lambda function to write log file records whenever a file is upload to the s3 bucket
