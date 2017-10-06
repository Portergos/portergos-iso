Ever need to install Antergos offline? With this ISO your needs are met!

This is an UNOFFICIAL iso. It’s build using mkarchiso and use both Antergos and Archlinux repositories

VERSION October 06th 2017
Download
iso http://www.mediafire.com/file/84mvipyn60i72tm/maroto-2017.10.06-x86_64.iso
md5sum http://www.mediafire.com/file/pig253x2c2iv23z/md5sum.txt

Purposes of the iso:

Easy experince using
i3-wm
Xfce4
Openbox
* The system will install the all 3 desktops
** At livecd, use "desktop switcher" at xfce4 panel to switch desktop (i3, openbox, xfce4) 

Ergonomic tools (easystroke)
Use Archlinux + Antergos repositories
Yaourt installed by default (AUR repositories)
Offline installer (modified from Pacbang linux) - Now also have online install options
Another online installer (Cnchi from Antergos)
Minimum systemd load after install (internet, cups, avahi, vboxservice and sddm) PC uses less ram memory
Use both iso/installed system as installer for others devices

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
Firejail (Opera and Firefox are set to start using firejail, changed in /usr/share/applications)

Games
Wine+Playonlinux
Steam

Scripts
scripts folder at ~/scripts
a) script clamav.sh

Script for using clamav, features are commented, you should open with any text editor and uncomment what you need. Every scan will generate a log for you to analyze the scan
Added update and scan at context menu from nemo

b) script xfce4.sh
My own script for starting and killing xfce4-panel (show/hide style, but using less resources)

c) Xfdesktop
dynamic menu (like xfce4 and openbox) using i3 shortcut $mod+x.
Very usefull to launch programs and logoff

d) Compressor
Created to use maximum compresison rate, you can choose 4 different methods (7z and tar.xz are the best)
Can be launched with alias "comp" in terminal or $mod+Ctrl+c under i3wm
Added at context menu from nemo also

e) Switch_session
Only for livecd. Use to switch desktop (i3, openbox, xfce4). Available at xfce4 panel.

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

Install ISO with it’s configs
Install from already installed USB/HD OR keep changed files
Online installer - Must edit packages_pacman.txt and packages_yaourt.txt at /abif-master
3.1) Use pacstrap only to download and install	
3.2) Use powerpill to download packages and pacstrap to install (Faster)
OBS2: It’s also possible to run Cnchi installer to have an Antergos desktop with it’s configs

You can run both offline and cnchi installers from the installed system, that means you can spread this OS system everywhere with a USB drive (when installed offline version)

OLD VERSIONS

VERSION September 12th 2017
Download
iso http://www.mediafire.com/file/5uukzc1j2b8i5id/maroto-2017.09.13-x86_64.iso
md5sum http://www.mediafire.com/file/yus4ykp4ahqd0p4/md5sum.txt

VERSION - August 17th 2017:
Download
iso http://www.mediafire.com/file/pbhj95o02b5fma1/maroto_1.1_cnchi_0.3_2017.08.17-x86_64.iso
md5sum http://www.mediafire.com/file/x5lw78qdg290gft/md5sum.txt

OLD VERSION (with pcmanfm bug and without cnchi installer):
Download
iso http://www.mediafire.com/file/a97am25wniffvr8/beta_1.1_maroto-2017.08.10-x86_64.iso
md5sum http://www.mediafire.com/file/o8i8rpqcce0eeig/md5sum.txt

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

Credits:

Developer and Maintainer: Fernando maroto

Antergos forum https://forum.antergos.com/topic/7655/unofficial-i3-wm-iso-with-offline-and-online-installer

More info at github https://github.com/marotinhodimais/Maroto-iso


Tester: Fernando maroto

Advisors: Joe Kamprad http://kamprad.net
          Velkerk

Also thanks to:
Keegan for uploading the iso at https://antergoscommunityeditions.wordpress.com/
Carl Duff for developing the first offline installer for Architect and PacBang (untill version 2.2.3 - 26-Mar-2016)
