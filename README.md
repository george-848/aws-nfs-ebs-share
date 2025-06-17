# aws-nfs-ebs-share
Set up NFS file sharing between two EC2 instances by mounting an EBS volume on the server and exporting it using NFS.

# AWS NFS Share with EBS and EC2

This project demonstrates how to share storage between two EC2 Linux instances using AWS EBS and NFS.

## Architecture
- **Server1**: EC2 instance with EBS volume attached and mounted  
- **Server2**: EC2 instance connected to the shared folder via NFS

## Steps Performed
1. Created and attached an EBS volume to Server1
2. Mounted the EBS volume to `/mnt/shared`
3. Installed and configured NFS on Server1 to export `/mnt/shared`
4. Configured Server2 to mount the NFS share
5. Verified read/write access across both instances

## Technologies
- AWS EC2
- EBS
- NFS
- Linux (Ubuntu)

## License
MIT
