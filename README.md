PORTERGOS (Portable Antergos) i3/Xfce4/Openbox - Offline/Online installer

![portergos_view](https://user-images.githubusercontent.com/18373928/34307317-ac1e4168-e72e-11e7-98b6-63afaf38c418.png)

EDIT November 30 2017 - I decided to rename the system to Portergos, sounds nice and cover it’s purpose.

Ever need to install Antergos offline? With this ISO your needs are met!

This is PORTERGOS (Portable Antergos). It’s build using mkarchiso and uses Portergos + Antergos + Archlinux repositories

VERSION November 30 2017
Download
iso https://github.com/Portergos/portergos-iso/releases/download/iso_02_12_2017/portergos-2017.12.02-x86_64.iso
md5sum https://github.com/Portergos/portergos-iso/releases/download/iso_02_12_2017/portergos-2017.12.02.md5sum

Purposes of the iso:

Easy experince using
i3-wm
Xfce4
Openbox

The system will install all 3 desktops
** At livecd, use “Oblogout” at xfce4 panel to switch desktop (close the session and login with wm of your choice)
Ergonomic tools (easystroke)
Use Portergos + Antergos + Archlinux repositories
Yaourt installed by default (AUR repositories)
Offline installer (modified from Pacbang linux) - Now also have online install options
Another online installer (Cnchi from Antergos)
Minimum systemd load after install (internet, cups, avahi, vboxservice and sddm) PC uses less ram memory
Use both iso/installed system as installer for others devices

GRUB better configurated after install wich has the following options:
Arch LTS kernel
Arch LTS kernel falback
Arch
Arch falback
Arch LTS - Terminal Login
reboot
poweroff

Themes
Arc-dark
Numix-solarized
Adapta-Nokto
AeeZee
Ambiant-Mate-Dark
Others

Icons
Vivacious
Zoncolor
Arc
Others

Security
ClamAV installed and some basic scripts for using it

Games
Wine+Playonlinux
Steam

Scripts
scripts folder at ~/scripts
a) script clamav

Script for using clamav, features are commented, you should open with any text editor and uncomment what you need. Every scan will generate a log for you to analyze the scan
Added update and scan at context menu from nemo

b) script xfce4
My own script for starting and killing xfce4-panel (show/hide style, but using less resources)

c) Xfdesktop
dynamic menu (like xfce4 and openbox) using i3 shortcut $mod+x.
Very usefull to launch programs and logoff

d) Compressor
Created to use maximum compresison rate, you can choose 4 different methods (7z and tar.xz are the best)
Can be launched with alias “comp” in terminal or $mod+Ctrl+c under i3wm
Added at context menu from nemo also

Others
Oblogout for logoff
Zim for notes
Redshift for eyes confort
Conky manager
Xed as text editor
Nemo as file manager (contains clamav script for update and scan)
Downgrader - Portergos repo
Caffeine-ng - Portergos repo

OBS1: Options inside offline installer

Install ISO with it’s configs (uses unsquashfs method, faster install)
Install from already installed USB/HD OR keep changed files
Online installer - Must edit packages_pacman.txt and packages_yaourt.txt at /abif-master
3.1) Use pacstrap only to download and install	
3.2) Use powerpill to download packages and pacstrap to install (Faster)
OBS2: It’s also possible to run Cnchi installer to have an Antergos desktop with it’s configs

You can run both offline and cnchi installers from the installed system, that means you can spread this OS system everywhere with a USB drive (when installed offline version)

It’s still under development, so use at your own risk. Also feel free to report bugs, needed packages, complains etc :p Made using the original archiso tool

More info
https://forum.antergos.com/topic/7655/unofficial-i3-wm-iso-with-offline-and-online-installer
My github @fernandomaroto under development https://github.com/marotinhodimais/Maroto-iso

@Keegan https://antergoscommunityeditions.wordpress.com/

@joekamprad http://kamprad.net/Downloads/

Post install

useful alias (located at /home folder)
Config files .bashrc and .zshrc contain two alias for updating the first time after install and in case of gpg errors, mirrorlist server down etc. (if you added your own user you should use sudo before the commands bellow)
To use key-init, refresh gpg signatures etc, just type:
up

Reflector to reorder the best servers, just type:
re

Or to do both just type:
u

TODO: Correct German translation (the current used an online translator English-German)
I’m currently packing some stuff i like and adding to repo, for example some themes that can be found on AUR and some only in the internet or other OSes.
Clean the installer and make it faster.

Credits:

Developer and Maintainer: Fernando maroto

Antergos forum https://forum.antergos.com/topic/7655/unofficial-i3-wm-iso-with-offline-and-online-installer

More info at github https://github.com/marotinhodimais/Maroto-iso

Tester: Fernando maroto

Advisors: Joe Kamprad http://kamprad.net
Velkerk

Also thanks to:
Keegan for uploading the iso at https://antergoscommunityeditions.wordpress.com/
Carl Duff for developing the first offline installer for Architect and PacBang (untill version 2.2.3 - 26-Mar-2016)
