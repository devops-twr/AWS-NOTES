# AWS-NOTES
Here you will get all aws steps
AWS EC2 NOTES DAY -1! 

EC2  --  Elastic  compute cloud

Amazon Elastic Compute Cloud (Amazon EC2) provides scalable computing capacity in the Amazon Web Services (AWS) cloud. 

Using Amazon EC2 eliminates your need to invest in hardware upfront, so you can develop and deploy applications faster. 

Synonyms

Computer, machine, box, PC, Server  = As per AWS terminology - Instance

Ex 1: Launch windows instnace

Step 1: Login to AWS 

Step 2: Choose region which is near ?  ( Asia pacific - Mumbai )

Step 3: Services --  EC2

	( If any keypairs -- delete )

	( If any security groups - delete,  except default )

	Services -- EC2 --- Launch Instance 

	Stage 1  -- Select AMI  ( Note: Select free tier eligible ) Win Server 2012

	Stage 2  --  t3.micro

	Stage 3   --  No of instances  --  1

	Stage 4  --  Storage - 30GB ( Observation - we have root - it is same as C Drive)

	Stage 5  --  Add Tag --  Giving name to the machine 

			Add Name Tag

			Value - MyWindows

	Stage 6  -- Security group  --  ( It deals with ports )

			We have 0 to 65535  ports

			Every port is dedicated to special purpose

			RDP -- 3389

			SSH -- 22

			HTTP -- 80

			HTTPS - 443


			For windows machine , we need to open RDP port  ( Remote Desktop Protocol )

			He by default , we have RDP


	Stage 7		Just observe the warnings, Just verify the options, Launch

Create a new keypair--  download key pair -- launch instance



We get the instance ID  i-0dddc6c37c9dfb460

			View Instances

Now, the new windows machines ,is having its own DNS Name, Username and password

We need to provide all the above 3 details in our laptop, so that we can connect.

We use an application called Remote Desktop Connection

AWS , gives us  DNS name , username, it does not give the password.

	Instead of password , AWS has given us pem file.

	But, to connect to Window, we need password

	AWS gives an option to convert .pem to password

How to connect .pem to password

---------------------------------

Connect to instance Get password -- upload pem file -- Decrypt  



Open Remote Desktop

Computer - Provide DNS

User name  --  Administrator

password  -- c&$*LjvfdL

Hurray!!

We are connected.





Lets check the hardware configuration

Check hard disk

Check Ram

You can copy paste file from laptop to win server  !!



To disconnect, just close the remote desktop window.

Explain about  Stop and reboot and terminate




++++++++++++++++END++++++++++++++++++++++++++++++++
