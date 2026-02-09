# AWS EC2 Windows VM Lab (RDP Access)

A beginner-friendly lab that walks through launching a Windows virtual machine in AWS and connecting to it securely via Remote Desktop (RDP).

## Watch me build this lab
https://loom.com/share/9a034b9d77f143d18157d71631305b02

**What this video shows:** Launching a Windows EC2 instance, creating a key pair, retrieving the Windows password, and connecting via RDP.

---

## Objective
Create and connect to a Windows virtual machine on AWS (EC2) so you have a working remote server environment for follow-on labs.

---

## Skills Practiced
- AWS EC2 instance provisioning
- Instance sizing and free-tier awareness
- Key pair creation and secure handling
- Basic networking/security review for remote access
- Instance health checks and status monitoring
- Windows password retrieval and decryption
- Remote Desktop (RDP) connectivity
- Cost-control habits (logging out / stopping when not in use)

---

## Tools Used
- AWS Management Console
- Amazon EC2
- Windows Server EC2 instance (example: Windows)
- Key pair file (PEM)
- Remote Desktop client (RDP)

---

## Steps Performed
## Creating a Virtual Machine in AWS

### Objective

This SOP outlines the steps to create and connect to a virtual machine in AWS, ensuring team members can execute the process efficiently.

### Key Steps

**Step 1: Access AWS and Launch Instances** [0:05](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=5)

![image alt](https://github.com/madebydxgxt/Cloud-Techniques/blob/main/Virtual-Machines/001/1.jpg?raw=true)



- Log in using your email.
- Wait for the dashboard to load.
- Click on 'Launch Instances' to start creating a new virtual machine.

**Step 2: Configure the Virtual Machine** [0:30](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=30)
![image alt](https://github.com/madebydxgxt/Cloud-Techniques/blob/main/Virtual-Machines/001/2.jpg?raw=true)

- Name your server (e.g., 'My Server 01').
- Select the type of virtual machine (choose Windows).
- Choose the instance type that fits within the free tier (e.g., 2 CPU, 8 GB memory).

**Step 3: Create a Key Pair** [1:25](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=85)
![image alt](https://github.com/madebydxgxt/Cloud-Techniques/blob/main/Virtual-Machines/001/3.jpg?raw=true)

- Select 'Create Key Pair'.
- Name your key pair (e.g., 'MyServerKey01').
- Click 'Create Key Pair' and ensure to download and save the key file securely.

**Step 4: Configure Network Settings** [2:20](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=140)
![image alt](https://github.com/madebydxgxt/Cloud-Techniques/blob/main/Virtual-Machines/001/4.jpg?raw=true)

- Leave the network settings as default.
- Click 'Launch Instance' to finalize the setup.

**Step 5: Monitor Instance Initialization** [3:10](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=190)
![image alt](https://github.com/madebydxgxt/Cloud-Techniques/blob/main/Virtual-Machines/001/5.jpg?raw=true)

- Go to 'Instances' to check the status of your new virtual machine.
- Wait until the status shows '3 out of 3 checks passed'.

**Step 6: Start the Instance** [3:50](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=230)
![image alt](https://github.com/madebydxgxt/Cloud-Techniques/blob/main/Virtual-Machines/001/6.jpg?raw=true)

- Select your virtual machine.
- Click on 'Instance State' and then 'Start Instance'.

**Step 7: Connect to the Instance** [4:21](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=261)
![image alt](https://github.com/madebydxgxt/Cloud-Techniques/blob/main/Virtual-Machines/001/7.jpg?raw=true)

- Once the instance is running, click on 'Connect'.
- Use the RDP client to connect.

**Step 8: Retrieve Password** [4:41](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=281)
![image alt](https://github.com/madebydxgxt/Cloud-Techniques/blob/main/Virtual-Machines/001/8.jpg?raw=true)

- Click on 'Get Password'.
- Upload the private key you downloaded earlier.
- Click 'Decrypt Password' and copy the generated password.

**Step 9: Download Remote Desktop File** [5:07](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=307)
![image alt](https://github.com/madebydxgxt/Cloud-Techniques/blob/main/Virtual-Machines/001/9.jpg?raw=true)

- Click on 'Download Remote Desktop File'.
- Open the downloaded file and enter the password when prompted.

**Step 10: Access the Virtual Machine** [5:44](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=344)
![image alt](https://github.com/madebydxgxt/Cloud-Techniques/blob/main/Virtual-Machines/001/10.jpg?raw=true)

- Click 'Yes' to connect to the virtual machine.
- Once connected, you can set up applications like Active Directory.

### Cautionary Notes

- Always save your key pair securely; losing it may prevent access to your virtual machine.
- Log out of your virtual machine when not in use to avoid unnecessary charges on your AWS account.

### Tips for Efficiency

- Familiarize yourself with the AWS interface to speed up the process.
- Keep a record of your key pairs and instance names for easy reference.


---

## Outcome
A Windows EC2 virtual machine was successfully launched and accessed via RDP using a decrypted administrator password, providing a ready server environment for additional lab work.
