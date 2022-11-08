## GraphGL
GraphGL is a RESTful application programming interfaces (API's) that enables you to access data globally service. 
After you register your app and get authentication tokens for a user or service, you can make requests to the GraphGL API's.

#### Information of systems components
```
Hardware Report:

Host Name:                 9F079636H
OS Name:                   Microsoft Windows 10 Pro
OS Version:                10.0.19043 N/A Build 19043
OS Manufacturer:           Microsoft Corporation
OS Configuration:          Standalone Workstation
OS Build Type:             Multiprocessor Free
Registered Owner:          {{users}}
Registered Organization:
Product ID:                00330-50000-00000-AAOEM
Original Install Date:     11/1/2022, 8:20:54 PM
System Boot Time:          11/7/2022, 1:51:51 PM
System Manufacturer:       TOSHIBA
System Model:              PORTEGE Z30-B
System Type:               x64-based PC
Processor(s):              1 Processor(s) Installed.
                           [01]: Intel64 Family 6 Model 61 Stepping 4 GenuineIntel ~2300 Mhz
BIOS Version:              TOSHIBA Version 6.50  , 3/6/2018
Windows Directory:         C:\Windows
System Directory:          C:\Windows\system32
Boot Device:               \Device\HarddiskVolume1
System Locale:             en-us;English (United States)
Input Locale:              en-us;English (United States)
Time Zone:                 (UTC+07:00) Bangkok, Hanoi, Jakarta
Total Physical Memory:     16,279 MB
Available Physical Memory: 7,268 MB
Virtual Memory: Max Size:  19,223 MB
Virtual Memory: Available: 10,034 MB
Virtual Memory: In Use:    9,189 MB
Page File Location(s):     C:\pagefile.sys
Domain:                    WORKGROUP
Logon Server:              \\9F079636H
Hotfix(s):                 6 Hotfix(s) Installed.
                           [01]: KB5018329
                           [02]: KB5000736
                           [03]: KB5012170
                           [04]: KB5018482
                           [05]: KB5018506
                           [06]: KB5001405
Network Card(s):           3 NIC(s) Installed.
                           [01]: Intel(R) Ethernet Connection (3) I218-LM
                                 Connection Name: Ethernet
                                 Status:          Media disconnected
                           [02]: Intel(R) Dual Band Wireless-AC 7265
                                 Connection Name: Wi-Fi
                                 DHCP Enabled:    Yes
                                 DHCP Server:     192.168.43.1
                                 IP address(es)
                                 [01]: 192.168.43.227
                                 [02]: fe80::3ce6:38e2:89da:add4
                           [03]: Hyper-V Virtual Ethernet Adapter
                                 Connection Name: vEthernet (WSL)
                                 DHCP Enabled:    No
                                 IP address(es)
                                 [01]: 172.25.48.1
                                 [02]: fe80::da63:18e9:fd8f:5ffc
Hyper-V Requirements:      A hypervisor has been detected. Features required for Hyper-V will not be displayed.
```
```
Software Report:

Server version:	Apache/2.4.54 (Win64)
PHP Version:	8.0.25 (cli) (built: Oct 25 2022 10:49:29) ( ZTS Visual C++ 2019 x64 )
Mysql Version:	Ver 15.1 Distrib 10.4.25-MariaDB, for Win64 (AMD64), source revision 23ddc3518f999e003d54f7a069b63b73585588aa
Laravel:	8.x Release September 8th, 2020
Laravel Octane:	Swoole application
```

#### Getting started for windows 10
- Settings > Apps and Features > Program and Features. Kemudian Klik Turn Windows Features on or off. checklist under `Windows Subsystem for Linux` and `Virtual Machine Platform`
- Windows Powershell
```
wsl --install `optional poin one`
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
systeminfo | find "System Type"
```
- download and install according to systeminfo
[x64](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) or [arm64](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_arm64.msi)
- Open the Microsoft Store application, then find the Linux system you want to install.
- Windows Powershell
```
wsl --set-default-version 2
wsl --list --verbose
```
- Open the Linux application that has been installed from the Microsoft Store application
