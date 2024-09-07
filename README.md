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



To set up an Application Load Balancer (ALB) in AWS, follow these steps:

1. Create Target Group
Open the AWS Management Console.
Navigate to the EC2 Dashboard.
Select Target Groups from the left-hand menu.
Click on Create target group.
Choose the target type: Instances, IP addresses, or Lambda function.
Enter a name for your target group.
Configure the protocol and port (e.g., HTTP, port 80).
Configure the VPC and health check settings.
Click Create.
2. Create an Application Load Balancer (ALB)
In the EC2 Dashboard, go to Load Balancers on the left-hand menu.
Click on Create Load Balancer and select Application Load Balancer.
Provide a name for your ALB.
Choose the scheme (Internet-facing or internal) based on your use case.
Select the IP address type (IPv4 or dual-stack).
Choose at least two Availability Zones and their corresponding subnets.
Under Security Groups, select an existing security group or create a new one to control traffic to the ALB.
In the Listeners section, choose the protocol and port (usually HTTP or HTTPS).
Click Next: Configure Routing.
3. Configure Listeners and Routing
Under Default action, choose Forward to and select the target group you created earlier.
If needed, configure advanced routing features like path-based or host-based routing.
Click Next: Register Targets.
4. Register Targets
Select the instances you want to register with the ALB from the target group.
Click Include as pending below.
Click Next: Review.
5. Review and Create
Review all your settings and configurations.
Click Create to set up your ALB.
6. Test the ALB
After creating the ALB, note its DNS name from the AWS console.
Use a browser or a tool like curl to send a request to the ALB's DNS name to verify that it is working as expected.
