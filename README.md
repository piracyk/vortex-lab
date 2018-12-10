# vortex-lab

**Indicator Netspeed** 

Unity is an Ubuntu AppIndicator which displays the current network upload / download speed on the panel.

**Usage

sudo apt-get install build-essential libgtop2-dev libgtk-3-dev libappindicator3-dev git-core
git clone https://github.com/GGleb/indicator-netspeed-unity.git
cd indicator-netspeed-unity
make
sudo make install
indicator-netspeed-unity &

**Deb

sudo apt-get install fakeroot dpkg-dev
delete line (	glib-compile-schemas $(DESTDIR)/usr/share/glib-2.0/schemas/ ) in Makefile
dpkg-buildpackage -rfakeroot -b

**PPA

sudo apt-add-repository ppa:fixnix/netspeed
sudo apt-get update
sudo apt-get install indicator-netspeed-unity

