# Kali NetHunter setup guide

You just flashed a NetHunter integrated kernel, and you wanna get Kali up and runnin'

Credits to [OffSec](https://offsec.com) for their amazing work

Let's get straight to it

# Installation

1 - Download the official [Kali NetHunter app store](https://store.nethunter.com/)

2 - Install it and enter, then download and install the following apps:

* NetHunter
* NetHunter Terminal
* NetHunter KeX

3 - Enter and enable all permissions and root access for NetHunter and NetHunter Terminal

## Configuring NetHunter

1 - Install the latest [kali-nethunter-rootfs-full-arm64.tar.xz](https://kali.download/nethunter-images/current/rootfs/)

2 - Enter NetHunter, open the sidebar, and navigate to Kali Chroot Manager

3 - Pick 'install from storage', and choose the downloaded `kali-nethunter-rootfs-full-arm64.tar.xz` file

4 - Wait for the installation to finish, and make sure your device stays ON/does not enter sleep mode during the chroot installation

5 - You now have Kali NetHunter fully running on your device, and you can configure chroot startup to your liking. You could also flash my firmware-fix module if you haven't already (required for supported USB WiFi adapter recognition)

## Configuring NetHunter KeX

1 - From NetHunter Terminal, run

`vncpasswd`

2 - Specify and verify your password (save it, as you'll need to input it again on NetHunter KeX)

3 - Then run

`vncserver :1`

It should show

`New Xtigervnc server 'localhost:1 (root)' on port 5901 for display :1.`

4 - Open NetHunter KeX, and fill the info as shown below

<img width="35%" alt="Screenshot_20260606-210349_NetHunter KeX_1" src="https://github.com/user-attachments/assets/1e67f94a-e8f0-4c9d-a724-49a31001cb55" />

Connect.

To turn off vncserver, navigate back to NetHunter Terminal and run

`vncserver -kill :1`

To shut down Kali NetHunter chroot completely, just navigate to Kali Chroot Manager in NetHunter app and press 'Stop' at the bottom

## Tested on

* Poco F4 GT (ingres)
* Android 16
* LineageOS 23.2
* Avalon Kernel

### If you need any help, you can [contact me](https://github.com/ruik3z) through my profile! Happy hunting!
