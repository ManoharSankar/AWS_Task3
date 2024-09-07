# AWS_Task
steps for s3bucket creation

Simple Storage Service
+++++++++++++++++++++++
-> S3 is object based storage

-> In s3 we can store all flat files 

-> We can upload, download and access files from S3

-> The files in s3 can't be executed

-> We can't install OS, DB etc in S3

-> We can't attach S3 to ec2 instance but we can access s3 data from EC2 instance

-> S3 is unlimited storage

-> S3 supports static website hosting 

-> S3 is cheaper than EC2 

-> S3 is serverless

-> In S3 we will store data in buckets. Bucket is a container. bucket contains object 

	Object = file
	key is name of the object
	
-> S3 is global but buckets are regional

-> Bucket names are universal and bucket name should be unique

Note: always create a bucket with your company name or project name.

-> We can't create one bucket inside another bucket

-> We can creat bultiple buckets in multiple regions

-> Max no.of buckets you can create in S3 is 100 (soft limit)

-> By default buckets are private, if required we can make it public.


Steps to create S3 Bucket
+++++++++++++++++++++++++++

-> Login into AWS Management Console

-> Go to S3 service

-> Click on Create Bucket
		
		- Choose Unique Name for Bucket

		- Select Nearest Region

		- Object Ownership : ACLs Enabled

		- Uncheck the checkbox of 'Block all public access'

		- Accept license agreement

		- Click on Create Bucket

