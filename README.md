dwm - dynamic window manager
============================
dwm is an extremely fast, small, and dynamic window manager for X.


Requirements
------------
In order to build dwm you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (dwm is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dwm (if
necessary as root):

    make clean install


Patches applied
---------------
* [dwm-6.0-winview.diff](https://dwm.suckless.org/patches/winview/dwm-6.0-winview.diff)
* [dwm-alpha-systray-6.3_full.diff](https://github.com/bakkeby/patches/blob/master/dwm/dwm-alpha-systray-6.3_full.diff)
* [dwm-attachbottom-6.3.diff](https://dwm.suckless.org/patches/attachbottom/dwm-attachbottom-6.3.diff)
* [dwm-barpadding-20211020-a786211.diff](https://dwm.suckless.org/patches/barpadding/dwm-barpadding-20211020-a786211.diff)
* [dwm-centeredmaster-6.1.diff](https://dwm.suckless.org/patches/centeredmaster/dwm-centeredmaster-6.1.diff)
* [dwm-doublepressquit-6.3.diff](https://dwm.suckless.org/patches/doublepressquit/dwm-doublepressquit-6.3.diff)
* [dwm-fancybar-20220527-d3f93c7.diff](https://dwm.suckless.org/patches/fancybar/dwm-fancybar-20220527-d3f93c7.diff)
* [dwm-fullgaps-6.4.diff](https://dwm.suckless.org/patches/fullgaps/dwm-fullgaps-6.4.diff)
* [dwm-gaplessgrid-20160731-56a31dc.diff](https://dwm.suckless.org/patches/gaplessgrid/dwm-gaplessgrid-20160731-56a31dc.diff)
* [dwm-hide_vacant_tags-6.3.diff](https://dwm.suckless.org/patches/hide_vacant_tags/dwm-hide_vacant_tags-6.3.diff)
* [dwm-movestack-20211115-a786211.diff](https://dwm.suckless.org/patches/movestack/dwm-movestack-20211115-a786211.diff)
* [dwm-noborder-6.2.diff](https://dwm.suckless.org/patches/noborder/dwm-noborder-6.2.diff)
* [overview](https://github.com/yaocccc/dwms/tree/1.3)
* [dwm-pertag-20200914-61bb8b2.diff](https://dwm.suckless.org/patches/pertag/dwm-pertag-20200914-61bb8b2.diff)
* [dwm-preview-all-windows-6.5.diff](https://github.com/luo216/preview-all-win/blob/master/dwm-preview-all-windows-6.5.diff)
* [dwm-restartsig-20180523-6.2.diff](https://dwm.suckless.org/patches/restartsig/dwm-restartsig-20180523-6.2.diff)
* [dwm-scratchpad-20221102-ba56fe9.diff](https://dwm.suckless.org/patches/scratchpad/dwm-scratchpad-20221102-ba56fe9.diff)
* [dwm-statuscmd-20241009-8933ebc.diff](https://dwm.suckless.org/patches/statuscmd/dwm-statuscmd-20241009-8933ebc.diff)
* [dwm-viewontag-20210312-61bb8b2.diff](https://dwm.suckless.org/patches/viewontag/dwm-viewontag-20210312-61bb8b2.diff)


Running dwm
-----------
Add the following line to your .xinitrc to start dwm using startx:

    exec dwm

In order to connect dwm to a specific display, make sure that
the DISPLAY environment variable is set correctly, e.g.:

    DISPLAY=foo.bar:1 exec dwm

(This will start dwm on display :1 of the host foo.bar.)

In order to display status info in the bar, you can do something
like this in your .xinitrc:

    while xsetroot -name "`date` `uptime | sed 's/.*,//'`"
    do
    	sleep 1
    done &
    exec dwm


Configuration
-------------
The configuration of dwm is done by creating a custom config.h
and (re)compiling the source code.


Overview
--------
![image](https://github.com/sl903dj/suckless/blob/statuscmd/2024-03-15_21-14.png)
![image](https://github.com/sl903dj/suckless/blob/statuscmd/2024-03-15_21-15.png)
