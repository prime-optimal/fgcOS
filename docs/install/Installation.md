---
created: 2023-04-23
updated: 2023-04-23 10:30
share: true
tags: Installation
---

### Step 1: Windows 10 Prep  
- Download Windows 10 stock ISO 
	- itechtips 
	- microsoft.com
- use Rufus to write the ISO to a flash drive 
	- Plug into USB 3.0 

> [!question]  Is this a success?
> Only time will tell.

```ad-tip
Copy the Atlas registry file to the USB drive.  Otherwise there will be additional services installed in the background the first time it connects to the internet
```

- Disable internet 
- Do video call
- Reboot 
- Press F11 to get into the BIOS select UEFI drive 
	- Custom Drive 
- Move old Windows install to Windows.old
	- Select Windows 10 install 
	- Do not connect to the internet 
	- Continue with limited setup
- Create user account and password 
- Click next 

```ad-warning
Make sure you're not connected to the internet before rebooting so it doesn't try to connect to install updates 
```

- Connect to the internet 
- Install AnyDesk for remote administration *not necessary for a self-install*
- Disable Windows Security Processes  
	- Windows Antivirus 
	- Real-time protection 
	- Cloud-delivered protection 
	- Automatic sample submission 
	- Tamper Protection 
- Run the Atlas registry file to disable Windows Update
	- disable driver update and windows update 
- Install Windows updates *don't do anything else while it's updating*

---

### Step 2: AtlasOS Install
- then install Atlas 
- AME Wizard 
- Run playbook file
- Reboots twice 
- then begin optimizing 

---

