## GraphGL
GraphGL is a RESTful application programming interfaces (API's) that enables you to access data globally service. 
After you register your app and get authentication tokens for a user or service, you can make requests to the GraphGL API's.

### Getting Started for Windows 10
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
