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
1. **Access AWS Console**  
   Logged into the AWS Management Console and navigated to EC2 to begin provisioning a new virtual machine.  
2. **Launch a new instance**  
   Started the EC2 “Launch Instance” flow to create a new virtual machine with standard AWS defaults.  
3. **Select Windows image**  
   Chose a Windows-based machine image to enable Remote Desktop access for a Windows server environment.  
4. **Choose an instance type**  
   Selected an instance size appropriate for learning and cost control (example: a free-tier-eligible option).  
5. **Create a key pair**  
   Created and downloaded a new key pair to securely retrieve/decrypt the Windows administrator password later.  
6. **Review networking and access**  
   Confirmed default networking settings and ensured remote access rules were appropriate (example: allow RDP from your IP).  
7. **Launch the instance**  
   Launched the virtual machine and let AWS begin provisioning and initializing the server.  
8. **Monitor instance health checks**  
   Verified the instance was fully initialized by checking that the system and instance status checks passed.  
9. **Confirm the instance is running**  
   Ensured the instance was in a running state (and started it if needed) before attempting to connect.  
10. **Retrieve and decrypt the Windows password**  
   Used the downloaded private key to decrypt the administrator password so the first login could be completed.  
11. **Connect using Remote Desktop**  
   Downloaded the RDP file (or used an RDP client), entered the decrypted password, and logged into the Windows VM.  
12. **Verify functionality and prep for next labs**  
   Confirmed you had interactive access to the desktop and the VM was ready for follow-on setup (example: installing roles like Active Directory).  
13. **Shut down safely to control costs**  
   Logged out and stopped (or terminated) the instance when finished to avoid unnecessary charges.  


---

## Outcome
A Windows EC2 virtual machine was successfully launched and accessed via RDP using a decrypted administrator password, providing a ready server environment for additional lab work.
