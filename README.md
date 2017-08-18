Hey all!

I'm very happy to announce my UNOFFICIAL iso. 

Purposes of the iso:

- Easy experince using i3-wm 
- Ergonomic tools (easystroke, lxsession, xfdesktop, xfce4-panel)
- Use Archlinux+Antergos+AUR repositories
- Offline installer (modified from Pacbang linux)
- Cnchi installer
- Minimum systemd load after install (internet, cups, avahi, vboxservice and sddm)
- Use both iso/installed system as installer for others devices

Security:

- ClamAV installed and some basic scripts for using it
- Firejail (Opera and Firefox are set to start using firejail, changed in /usr/share/applications)

Games

- Wine+Playonlinux
- Steam

Others

- Oblogout for logoff
- Zim for notes
- Redshift for eyes confort
- Conky manager
- Others

NEW VERSION - August 17th 2017
Changes:
1) Added a new option inside the offline installer (Keep changes made while running the iso, and also used to install from installed system like USBs to another hd or USB)
2) Added Cnchi (everthing seems to work, i just removed the zfs support, and Antergos' wallpapers are not installed in the new system)
3) `xed` as new text editor replacing gedit (also tested leafpad and mousepad, xed is the big winner)
4) `caja` as new file manager replacing pcmanfm
*pcmanfm was buggy, and caja does what i need (F3 option to split pane and "open terminal here", also matches perfectly fine with the theme)
5) Resolution 1280x720 not automatically at startup, you can change using $mod+p (since you can change in VB options as well) System starts with 800x600
6) You can run both offline and cnchi installers from the installed system, that means you can spread this OS system everywhere with a USB drive :P 

Download links 
direct link
http://www.mediafire.com/file/pbhj95o02b5fma1/maroto_1.1_cnchi_0.3_2017.08.17-x86_64.iso

md5sum
http://www.mediafire.com/file/x5lw78qdg290gft/md5sum.txt

Old version (with pcmanfm bug and without cnchi installer):
direct link
http://www.mediafire.com/file/a97am25wniffvr8/beta_1.1_maroto-2017.08.10-x86_64.iso

md5sum
http://www.mediafire.com/file/o8i8rpqcce0eeig/md5sum.txt

It's still under development, so use at your own risk.
Also feel free to report bugs, needed packages, complains etc :p 
Made using the original archiso tool 

More info
My github @fernandomaroto under development
https://github.com/marotinhodimais/Maroto-iso

@Keegan 
https://antergoscommunityeditions.wordpress.com/

@joekamprad 
http://kamprad.net/Downloads/
