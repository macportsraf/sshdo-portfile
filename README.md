# README

My version of my sshdo macports Portfile.

It differs from the official Portfile in that it uses whatever python or
python3 is already available, rather than requiring a port of a particular
version of python that requires it to be updated every year or so. And it
includes all four download sites, rather than just one.

Actually, there is still no official Portfile for sshdo. It's been waiting
months to be merged. Perhaps it never will be.

# INSTALL

You need your own set of ports to install this from:

    cd ~/src
	git clone https://github.com/macportsraf/sshdo-portfile
	mkdir ~/ports
	cp -pr sshdo-portfile/security ~/ports
	rm -rf sshdo-portfile
	cd ~/ports
	portindex
	echo file://$(pwd) >> /opt/local/etc/macports/sources.conf

