# How to Setup ec2

step 1: Go to AWS CONSOLE.Then go to services in the menu bar.

step 2: select EC2 from compute section or you can search for 'ec2' in search bar.
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20181107.png)

step 3: Click on 'launch instance'.
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20181354.png)	

step 4: Select which AMI You want from the list or ypu can search for AMI from search bar.
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20181430.png)	

step 5: select instance type. You can choose family of instance type according to your CPU and Memory requirements.
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20181449.png)	

step 6: Click on 'next:Configure Instance details' if you want any changes in the default configurations.
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20181520.png)	


step 7: After configuration setting now you can change storage details according to your requirements.
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182235.png)	


here you can see i have changed the size of the storage to 30 as per my requirements. now you click on 'next:add tags'.

step 8: Here You can add tag to to your instances.so click on 'Add tag'.write name in key box and value can be any name as per your choice.
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182312.png)	


now click on 'Next:configure security groups.But before that let's understand what is security group.

Security Group
A security groups acts as a virtual firewall similar like windows firewall that controls the traffic for one or more instances.
When we launch (create) an instance, we can specify one or more security groups or we can use the default security group provided by aws.
security group has inbound and outboud rules which controls incoming and outgoing traffic by enabling/disabling ports respectively.
step 9: so now you can create new security group and enter the security group name and description or you can select exsting security groups.
image

now click on you can click on 'review and launch'.

![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182436.png)	


here you will see all your ec2 instance configurations you have choosen.If you want to change some conguration you can click on previous till you go to the page where you want to make any changes.

step 10: now you can click on launch.now you will get window for selecting or creating key pair.before that let's understand what is key pair,
A key pair consists of a public key that AWS stores, and a private key file that you store. Together, they allow you to connect to your instance securely. For Windows AMIs, the private key file is required to obtain the password used to log into your instance. For Linux AMIs, the private key file allows you to securely SSH into your instance.

you can select existing key pair or create new key pair.here we are creating new key pair.so select 'create new key pair' from dropdown and give name to the key pair.

![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%201822.png)	


step 11: Click on download key pair.it is important to download the key pair pem file.it will need to create ssh for you instance.
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182235.png)	

step 12: now click on launch instance.

![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182235.png)	


done...you can see you instance which can be like your laptop which is created in hardly 10 minutes.

here you can see your instance creation status.

now you can click on view instance list.and now yon are able to see the instance list.

![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182235.png)	


step 13: now you can change your instance state by selecting instance then click on 'Actions' in the menu,now select 'stance state' from the options.
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182235.png)	


Instance states:

start: if your instance is in the stopped state you can again state by selecting start state.
stop: if you dont have use of your current instance you can stop it so it will affect on your cost which you are paying for your instance.for stopped instance you are only paying for your storage spcae and not for CPY and MEMORYY.
Terminate:you can permanently delete your instance by changing to this state.
