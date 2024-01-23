Bootstrap: docker
From: ubuntu:16.04

%post
apt-get -ymq update
apt-get -y install firefox python3 python3-pip wget curl git python3-dbus python3-pyinotify \
python3-xlib wmctrl python3-packaging autokey-gtk grabc zip fuse xterm xvt x11-apps xdotool

##grab the firefox add-on
#rm -rf /tmp/moz_extensions_tmp
#mkdir -p /tmp/moz_extensions_tmp
#cd /tmp/moz_extensions_tmp
#wget https://addons.mozilla.org/firefox/downloads/file/3777751/rpa-6.2.6.xpi
#unzip rpa-6.2.6.xpi
#
#EXTENSION_STRING=$(echo `grep id manifest.json | cut -d ':' -f 2 | tr -d '/"/'`)
#mkdir -p /usr/lib/firefox-addons/extensions/${EXTENSION_STRING}/
#mv rpa-6.2.6.xpi /usr/lib/firefox-addons/extensions/${EXTENSION_STRING}/rpa-6.2.6.xpi
#
#
#### get appimage for xmodules
#mkdir -p /opt 
#
#cd /tmp
#
#wget https://download.ui.vision/x/uivision-xmodules-linux-v2.AppImage
#chmod a+x uivision-xmodules-linux-v2.AppImage
##
#./uivision-xmodules-linux-v2.AppImage --appimage-extract
#more needs to be added to address issues with glibc
%environment
export LC_ALL=C

%runscript
