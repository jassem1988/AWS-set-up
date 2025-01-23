# AWS-set-up

## Objective
Setting up a AWS account and creating EC2.

### Skills Learned

- Creating EC2
- SSH
- EBS Volume
  

### Tools Used

- AWS Cloud Computing

### Steps to create a new EC2 instance
1. Login to your AWS account and then search for EC2 or use the menu
   
<img width="414" alt="image" src="https://github.com/user-attachments/assets/bc34087f-fc1a-4c97-8973-963645716cc1" />

3. Click on launch instance to create a new instance

<img width="363" alt="image" src="https://github.com/user-attachments/assets/717a6592-3172-41e7-b5e2-2bf4d8ea9d10" />

4. Create a name for your instance and then choose an OS image AMI (Amazon Machine Image) and choose the instance type
   
<img width="977" alt="image" src="https://github.com/user-attachments/assets/b968ab32-1ef8-4766-a699-aaf2144700fa" />

6. Create a key pair and download it to your computer
   
<img width="611" alt="image" src="https://github.com/user-attachments/assets/858905e2-549e-4053-8639-026954661fec" />

8. Set up the firewall (security groups) and allow SSH and then launch the instance
   
<img width="611" alt="image" src="https://github.com/user-attachments/assets/f7616da1-7d46-4535-b09b-c7b248270e02" />

10. Open terminal (Mac) and type
```bash
% sudo chmod 400 ~/Desktop/jassem_test.pem
```
>The location of your private key
7. Then you will connect to the instance via SSH
```bash
ssh -i ~/Desktop/jassem_test.pem ubuntu@(MAC address of the instance)
```
>Make sure to type the right username for the right AMI
8. Then you type you Mac password and agree to the question and then you will be connected to your Instance
<img width="725" alt="image" src="https://github.com/user-attachments/assets/a76fa3c7-c580-4756-98d9-fbb377583d18" />

### Step to create a EBS Volume and attach it to an instance EC2

1. We create a new volume from the menu
   
<img width="762" alt="image" src="https://github.com/user-attachments/assets/c5451ebb-f4db-4d37-ae53-52f9e217e0bf" />

2. We choose a size for the EBS Volume and choose to be encrypted or not

<img width="580" alt="image" src="https://github.com/user-attachments/assets/6f3c6f80-7dd2-4b40-b8d2-3cc159a26030" />

3. Add a tag and name it

<img width="936" alt="image" src="https://github.com/user-attachments/assets/2351a485-0716-4ce7-a992-475ba0fe842f" />






