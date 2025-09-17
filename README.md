# sysadmin-cloud-vhd-migration
Converts VirtualBox VDI images to Azure-compatible VHDs and uploads them to Azure Blob Storage. Includes Windows Server 2022, Ubuntu Server, and Kali Linux. Part of my SysAdmin Bootcamp lab project (https://github.com/rippey81/sysadmin-lab)  for learning cloud migration and virtualization.

---

# ☁️ SysAdmin Lab – Local to Azure Cloud Migration

## 🔧 Objective

Convert locally hosted VirtualBox VMs (`.vdi`) into Azure-compatible `.vhd` format and upload them to Azure Blob Storage for VM creation and cloud-based lab accessibility.

## 💻 Local Environment

- **Host OS:** Windows 10  
- **VirtualBox VMs:**
  - Windows Server 2022  
  - Ubuntu Server  
  - Kali Linux  

## ⚙️ Tools Used

- Oracle VirtualBox  
- Command Prompt (`VBoxManage`)  
- Azure Portal  
- Azure Storage Explorer  
- GitHub  

## 🧱 Steps Taken

### 1. Convert VDI to VHD

```bash
VBoxManage clonehd "C:\path\to\VM.vdi" "C:\path\to\VM.vhd" --format VHD
```

### 2. Upload to Azure

- Installed Azure Storage Explorer

- Signed in using Azure for Students subscription

- Created a Blob Container in a Storage Account

- Uploaded .vhd files to Blob storage

### 3. Next Steps

- Convert uploaded .vhd into Managed Disks

- Deploy Azure VMs from Managed Disks

- Configure networking, remote access (RDP/SSH)

- Begin cloud-based lab operations and testing

## 📚 Why This Matters

This migration project bridges traditional sysadmin training with cloud infrastructure (IaaS). It demonstrates:

- Proficiency with virtual machine formats & disk image conversion

- Hands-on use of Azure Storage and VM creation workflows

- Practical hybrid cloud skills vital for modern sysadmins

## 🧠 Lessons Learned

- Differences between .vdi and .vhd formats

- Troubleshooting disk size & VERR_DISK_FULL errors

- Navigating Azure Blob storage and understanding containers

- Real-world file system management during constrained local disk space

- The importance of cloud-readiness and backup migration options

## 🚀 This lab is part of the Sysadmin-Lab project (https://github.com/rippey81/sysadmin-lab) to showcase hands-on experience in enterprise and cloud infrastructure.
