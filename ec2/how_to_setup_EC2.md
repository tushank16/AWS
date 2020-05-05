# How to Setup EC2

**Step 1: Go to AWS CONSOLE.Then go to services in the menu bar.**

**Step 2: Select EC2 from compute section or you can search for 'ec2' in search bar.**
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20181107.png)

**Step 3: Click on *'launch instance'*.**
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20181354.png)	

**Step 4: Select which AMI You want from the list or ypu can search for AMI from search bar.**
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20181430.png)	

**Step 5: Select instance type. You can choose family of instance type according to your CPU and Memory requirements.**
* It will also show the cpu configeration and other details.
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20181449.png)	

**step 6: Click on next:*'Configure Instance details'* if you want any changes in the default configurations.**
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20181520.png)	
> Here *Advance details* -> *user data* you can add a file at the time of creating an instance 
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182235.png)	


**Step 7: After configuration setting next is *Add Storage*.**
* Here you can change the size of the storage to as per your requirements. now you click on 'next:add tags'.

![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182312.png)	

**Step 8: Here You can add tag to to your instances.so click on 'Add tag'.write name in key box and value can be any name as per your choice.**


>Now click on 'Next:configure security groups.But before that let's understand what is security group.

## **Security Group**
* A security groups acts as a virtual firewall similar like windows firewall that controls the traffic for one or more instances.
* When we launch (create) an instance, we can specify one or more security groups or we can use the default security group provided by aws.
* Security group has inbound and outboud rules which controls incoming and outgoing traffic by enabling/disabling ports respectively.

**Step 9: Configuring security groups**
* Now you can create new security group and enter the security group name and description or you can select exsting security groups.
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182436.png)	

now click on you can click on 'review and launch'.
- *Review Instance Launch*
![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182454.png)	

- Here you will see everything as a preview before you confirm .You can view your ec2 instance configurations what you have choosen.If you want to change some conguration you can click on previous till you go to the page where you want to make any changes.

**Step 10: Selecting key pair for instance login**

After clicking on launch. Now you will get window for selecting or creating key pair.before that let's understand what is key pair,
- A key pair consists of a public key that AWS stores, and a private key file that you store. 
- Together, they allow you to connect to your instance securely. 
- For Windows AMIs, the private key file is required to obtain the password used to log into your instance. 
- For Linux AMIs, the private key file allows you to securely SSH into your instance.
- You can select existing key pair or create new key pair.here we are creating new key pair.so select 'create new key pair' from dropdown and give name to the key pair.
- Without a key it is imposible to login to your instance

![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182511.png)	


**Step 11: Click on download key pair.**

![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182550.png)	
- It is important to download the key pair pem file.it will need to create ssh for you instance.
- Without downloading key pair you cannot click on launch instance.

**Step 12: Click on launch instance.**

![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182620.png)	
- You can see you instance which can be like your laptop which is created in hardly 5 minutes.

CLICK ON VIEW INSTANCE TO VIEW IT.

![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182640.png)	

- Here you can see your instance creation status.

- Now you can click on view instance list.and now yon are able to see the instance list.

![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182740.png)	


**Step 13: now you can change your instance state by selecting instance then click on 'Actions' in the menu,now select 'instance state' from the options.**

![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182800.png)	

- You can see the instance state is running.

**Viewing volume**
* Click on Elastic block -> Volumes , to view the volume(memory).

![Image](https://github.com/tushank16/AWS/blob/aws_services/ec2/images/Annotation%202020-05-05%20182957.png)	

## Instance states:

- **Start:** if your instance is in the stopped state you can again state by selecting start state.
- **Stop:** if you dont have use of your current instance you can stop it so it will affect on your cost which you are paying for your instance.for stopped instance you are only paying for your storage spcae and not for CPY and MEMORYY.
- **Terminate:** you can permanently delete your instance by changing to this state.
