# AWS EC2 + EBS Persistent Storage Deployment

## Project Overview
This project demonstrates the deployment and validation of persistent block storage on an Amazon EC2 Linux instance using Amazon Elastic Block Store (EBS). The implementation includes Linux filesystem creation, permanent mount configuration, reboot persistence testing, and deployment verification.

---

## Objectives
- Launch and validate Amazon EC2 compute environment
- Attach and identify secondary EBS volume
- Create Linux EXT4 filesystem on attached block storage
- Configure persistent mount point using /etc/fstab
- Validate automatic remount after system reboot
- Document command execution and deployment evidence

---

## AWS Services Used
- Amazon EC2
- Amazon Elastic Block Store (EBS)
- EC2 Instance Connect
- Linux Filesystem Utilities

---

## Deployment Steps Performed
1. Verified attached EBS block device using lsblk
2. Created mount directory /data
3. Formatted EBS volume with EXT4 filesystem
4. Retrieved UUID using blkid
5. Configured /etc/fstab for persistent mounting
6. Executed sudo mount -a validation
7. Confirmed mounted filesystem using df -h
8. Created persistence test file
9. Rebooted instance and validated storage retention

---

## Validation Evidence
Deployment validation includes:
- Successful /data mount confirmation
- Persistent file retention after reboot
- AWS instance running state verification
- Linux command execution documentation

See:
- commands-used.txt
- architecture-notes/deployment-summary.txt
- screenshots/

---

## Key Outcome
Successfully implemented enterprise-style persistent storage attachment to cloud compute resources while demonstrating Linux systems administration, AWS infrastructure management, and deployment persistence validation.

---

## Author
Ivan Garcia 
Cloud Engineering / AWS Hands-On Portfolio Project
