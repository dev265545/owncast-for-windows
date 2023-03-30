# Owncast-for-windows

> Note:  Owncast currently **does not support Windows Operating System**. This is a workaround to run Owncast on Windows.


This document list out the steps in detail to install and run Owncast in Windows using Windows Subsystem for Linux, specifically **WSL2**

---

### Step 1 : Installing WSL2 in Windows.
There are lots of tutorial available online (videos and docs both) on how to install WSL2.  
Here are the official documents from Microsoft -> [Install Linux on Windows with WSL](https://learn.microsoft.com/en-us/windows/wsl/setup/environment)
Some points to remember -> 
- Preferable method to install WSL2 is by using  the `wsl --install `. If you are facing issues with this method you can look at - [Manual installation steps for older versions of WSL](https://learn.microsoft.com/en-us/windows/wsl/install-manual)
- Make sure you have enabled Virtual Machine feature. (ignore if used wsl --install method)
- Make sure you have WSL2
- Installed your Linux distribution of choice and make sure you installed the latest avaiable version (Preferably Ubuntu)


### Step 2 : Setting up WSL2 and the distribution of your choice.


`ip addr show eth0 | grep -oP '(?<=inet\s)\d+(\.\d+){3}'`
`wsl -- ip -o -4 -json addr list eth0`
