This is an UNOFFICIAL iso. It's build using mkarchiso and use both Antergos and Archlinux repositories

VERSION September 12th 2017
Download
iso http://www.mediafire.com/file/5uukzc1j2b8i5id/maroto-2017.09.13-x86_64.iso
md5sum http://www.mediafire.com/file/yus4ykp4ahqd0p4/md5sum.txt

Purposes of the iso:

- Easy experince using i3-wm (lxsession, xfdesktop, xfce4-panel)
- Ergonomic tools (easystroke)
- Use Archlinux + Antergos repositories
- Yaourt installed by default (AUR repositories)
- Offline installer (modified from Pacbang linux) - Now also have 2 online install options
- Online installer (Cnchi from Antergos)
- Minimum systemd load after install (internet, cups, avahi, vboxservice and sddm) PC uses less ram memory
- Use both iso/installed system as installer for others devices

Theme
arc-icon-theme
gtk-theme-numix-solarized

Security
ClamAV installed and some basic scripts for using it
Firejail (Opera and Firefox are set to start using firejail, changed in /usr/share/applications)

Games
Wine+Playonlinux
Steam

Others
Oblogout for logoff
Zim for notes
Redshift for eyes confort
Conky manager
Xed as text editor
Nemo as file manager (contains clamav script for update and scan)
Downgrader - AUR repo
Caffeine-ng - AUR repo

OBS1: Options inside offline installer
1) Install ISO with it's configs
2) Install from already installed USB/HD OR keep changed files
3) Online installer - Must edit packages_pacman.txt and packages_yaourt.txt at /abif-master 
    3.1) Use pacstrap only to download and install	    
    3.2) Use powerpill to download packages and pacstrap to install (Faster)

OBS2: It's also possible to run Cnchi installer to have an Antergos desktop with it's configs

You can run both offline and cnchi installers from the installed system, that means you can spread this OS system everywhere with a USB drive

OLD VERSIONS
VERSION - August 17th 2017:
Download 
iso http://www.mediafire.com/file/pbhj95o02b5fma1/maroto_1.1_cnchi_0.3_2017.08.17-x86_64.iso
md5sum http://www.mediafire.com/file/x5lw78qdg290gft/md5sum.txt

OLD VERSION (with pcmanfm bug and without cnchi installer):
Download
iso http://www.mediafire.com/file/a97am25wniffvr8/beta_1.1_maroto-2017.08.10-x86_64.iso
md5sum http://www.mediafire.com/file/o8i8rpqcce0eeig/md5sum.txt

It's still under development, so use at your own risk. Also feel free to report bugs, needed packages, complains etc :p Made using the original archiso tool

More info 
https://forum.antergos.com/topic/7655/unofficial-i3-wm-iso-with-offline-and-online-installer
My github @fernandomaroto under development https://github.com/marotinhodimais/Maroto-iso

@Keegan https://antergoscommunityeditions.wordpress.com/

@joekamprad http://kamprad.net/Downloads/


Post install

1) useful alias (located at /home folder)
Config files .bashrc and .zshrc contain two alias for updating the first time after install and in case of gpg errors, mirrorlist server down etc. (if you added your own user you should use sudo before the commands bellow)

To use key-init, refresh gpg signatures etc, just type: 
up

Reflector to reorder the best servers, just type: 
re

Or to do both just type:
u

2) scripts folder at ~/scripts

a) script clamav.sh

My own script for using clamav, features are commented, you should open with any text editor and uncomment what you need. Every scan will generate a log for you to analyze the scan.

b) script xfce4.sh
My own script for starting and killing xfce4-panel (show/hide style, but using less resources)

c) Xfdesktop
Is a package to manage desktop (show icons at desktop). You can use for this purpose but won't work very well under i3-wm
dynamic menu (like xfce4 and openbox) using i3 shortcut $mod+x.
Very usefull to launch programs and logoff.
