### Kali NetHunter setup guide

You just flashed a NetHunter integrated kernel, and you wanna get Kali up and runnin'

Credits to [OffSec](offsec.com) for their amazing work

Let's get straight to it

## Installation

1 - Download the official [Kali NetHUnter app store](https://store.nethunter.com/)

2 - Install it and enter, then download and install the following apps: NetHunter, NetHunter Terminal, NetHunter KeX

3 - Enter and enable all permissions and root access for NetHunter and NetHunter Terminal

### Configuring NetHunter

1 - Install the latest [kali-nethunter-rootfs-full-arm64.tar.xz](https://kali.download/nethunter-images/current/rootfs/)

2 - Enter NetHunter, open the sidebar, and navigate to Kali Chroot Manager

3 - Pick install from storage, and choose the downloaded 'kali-nethunter-rootfs-full-arm64.tar.xz' file

4 - Wait for the installation to finish, and make sure your device stays ON/does not enter sleep mode during the chroot installation

5 - You now have Kali NetHunter fully running on your device, and you can now configure chroot startup to your liking. You could also flash my firmware-fix module if you haven't already (required for USB WiFi adapter recognition)

### Configuring NetHunter KeX

1 - From NetHunter Terminal, run
`vncpasswd`

2 - Specify and verify your password

3 - Then run
`vncserver :1`

It should show
`New Xtigervnc server 'localhost:1 (root)' on port 5901 for display :1.`

4 - Open NetHunter KeX, and fill the info as shown below. Then Connect

To turn off vncserver, navigate back to NetHunter terminal and run
`vncserver -kill`

To shut down Kali NetHunter chroot completely, just navigate to Kali Chroot Manager in NetHunter app and press 'Stop' at the bottom

## If you need any help, you can contact me through my [profile](https://github.com/ruik3z)! Happy hunting!
