rpm-keepalived
==============

An RPM spec file build and install keepalived.

To Build:

`sudo yum -y install rpmdevtools && rpmdev-setuptree`

`sudo yum -y install openssl-devel kernel-devel`

`wget http://www.keepalived.org/software/keepalived-1.2.7.tar.gz -O ~/rpmbuild/SOURCES/keepalived-1.2.7.tar.gz`

`wget https://raw.github.com/nmilford/rpm-keepalived/master/keepalived.spec -O ~/rpmbuild/SPECS/keepalived.spec`

`rpmbuild -bb ~/rpmbuild/SPECS/keepalived.spec`