---
share: true
---
### Step 3: Optimizations
#### Atlas Shortcuts
- Winrar 
- Brave
- Atlas Folder -> Advanced Configuration -> NVIDIA Display Container -> Disable Container 
  ![[2023-04-22-17-32-15 1.png]]
  	- Check Display Settings to verify refresh rate 
	- Configuration -> General Config -> Disable **Most**
		- General Config -> Mitigations -> Disable All Mitigations disables spectre and meltdown which introduce latency.  *Secure Boot must be off* 
		- Start Menu 
			- Install OpenShell 
	- Disable VPN  
- 
- Install Drivers 
	- Realtek Audio Drivers 
	- Ethernet LAN Drivers 
	- GPU Drivers 
		- Discreet GPU drivers install (NVIDIA or AMD)
			- NVCleanInstall  *automatically selects the driver version and you can turn off telemetry*
				- Disable Telemetry 
				- Perform clean installation 
				- Expert Tweaks 
					- Disable Telemetry 
					- Enable Mesage Signal  interrupts 
					- Disable HDCP 
					- Apply NVENC Video Encoding 
			- NVIDIA Control Panel 
				- Manage 3D Settings ![[Pasted image 20230422172249.png]]
					- High performance NVIDIA Processor 
				- Low Latency Mode - **Ultra** 
				- Power Mode - **Maximum performance** 
				- Vertical Sync - **Off**
		- Integrated GPU drivers (Intel)
- Custom Resolution Utility (CRU)
- Display Settings
	- Verify refresh rate of the monitor 

##### Do Not Disable
- Xbox 
- UWP 
- UAC 
- Wi-Fi
- Windows Firewall
- Microsoft Store 
- FSO and Game Bar 

##### Optional
Some games come with these already, but it's likely these will need to be installed.
- Visual C++ Redistributable
- Visual .NET Redistributable 


```ad-tip
At this point there should probably be around ~60 processes 
```

- GameUtil - *kills desktop window manager which removes 1 frame of lag, locks*  
	- Move to desktop
	- go to gameutil first then load game
	- Disable Idle
- LatencyMon
- Install Steam
	- Login and start downloading game 
	- Configure controller 
	- Install games 
	- Right click the steam shortcut -> Properties and enter this command:

```
"C:\Program Files (x86)\Steam\Steam.exe" -no-browser +open steam://open/minigameslist
```

- Intelligent Standby List Cleaner 
- Install MSI Tool 
	- https://forums.guru3d.com/threads/windows-line-based-vs-message-signaled-based-interrupts-msi-tool.378044/


#### Calypto's Latency Guide (calypto.us)
- Open Powershell in Administrator Mode 
- bcedit /set disabledynamictick yes 
- Device Manager 

#### Melody Low Latency Script 
- Basic Tweaks 
- bcedit commands

```ad-note
Add Melody tweak commands here 
```

#### fgcOS Tweaks 

- [Peace Equalizer](https://sourceforge.net/projects/peace-equalizer-apo-extension/) 
- [Equalizer APO](https://sourceforge.net/projects/equalizerapo/)
	![[Pasted image 20230422181519.png]]
- Special K 
	- Turn on Latent Sync 
	- Delay Bias: All Input No Display
	- Add Fightcade 
		- emulator -> FBNeo
		- c:\$USERDIRECTORY$\Documents\Fightcade\emulator\fbneo\roms
	- CTRL+SHIFT+ESC 
		- File -> Install Wrapper DLL 
		- Framerate limit (right click turn on Latent Sync)
	- You can tell it's injecting when the UI turns blue 
	- Adaptive Sync **off** 
	- All Input No Display 
	- Turn off OSD 
- hidusbf
	- Inside the folder, install the sweetlow certificate 
	- Enable each controller by clicking Install Service, Filter on Device, set polling to 1000.
- DS4 Windows 
- [ISLC](https://www.wagnardsoft.com/forums/viewtopic.php?t=1256)
	![[Pasted image 20230422185034.png]]
- OBS Settings *optional*


---

### Step 4: Game-Specific Optimizations 
- Graphic settings for each game 
- Disable V-Sync 

#### Fightcade
- DirectX drivers 
- Configure controller
- FC2JSON Pack 
	- ##### 3rd Strike 
		- [PalMod](https://zachd.com/palmod/releases/) *color palette mods* 
		- [re:THIRD 3rd Strike color palettes, HUD, and stage mods](https://www.youtube.com/watch?v=4THUKhm3CnE) | [Download](https://mega.nz/file/xV9RzSAb#k8VztZl8WxI-hYQdz45LcToSj4W_4tQV42-y18lvlz4)
		- [3rd Strike Training Mode script](https://github.com/Grouflon/3rd_training_lua) 

##### Troubleshooting
- Disable Special K 
- Reduce Latent Sync from 100% to **50% Input, 50% Display** and then adjust accordingly.
- Make sure the frame display counter is on. 

#### Tekken 7
- Tekken Overlay  
#### Street Fighter V 
- 

#### DragonBall FighterZ
- 

#### King of Fighters XV
- Troubleshooting: You might need the Visual C++ Redistributable 
- [Disable V-Sync](https://whatifgaming.com/how-to-enable-the-king-of-fighters-xv-vsync-option-on-pc/) 


---
### Step 5: Customization, Troubleshooting, and Edge Cases 

### Microsoft Services to Potentially Disable 
- Windows Font Cache Service 
- Windows Push Notifications 
- Touch Keyboard and Handwriting Panel Service 
- Sync Host 
- User Data Storage 

#### GameUtil 

#### Special K
- This has to be optimized for each game individually. 
- 
