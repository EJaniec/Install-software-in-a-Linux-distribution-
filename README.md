# Install-software-in-a-Linux-distribution-

  install - install packages
  reinstall - reinstall packages
  remove - remove packages
  autoremove - Remove automatically all unused packages
  update - update list of available packages
  upgrade - upgrade the system by installing/upgrading packages
  full-upgrade - upgrade the system by removing/installing/upgrading packages
  edit-sources - edit the source information file

See apt(8) for more information about the available commands.
Configuration options and syntax is detailed in apt.conf(5).
Information about how to configure sources can be found in sources.list(5).
Package and version choices can be expressed via apt_preferences(5).
Security details are available in apt-secure(8).
                                        This APT has Super Cow Powers.
analyst@e980ac1fd1be:~$ sudo apt install suricata
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following additional packages will be installed:
  geoip-database libauthen-sasl-perl libdata-dump-perl libencode-locale-perl libevent-2.1-6 libevent-core-2.1-6 libevent-pthreads-2.1-6 libfile-listing-perl libfont-afm-perl libgeoip1 libhiredis0.14
  libhtml-form-perl libhtml-format-perl libhtml-parser-perl libhtml-tagset-perl libhtml-tree-perl libhtp2 libhttp-cookies-perl libhttp-daemon-perl libhttp-date-perl libhttp-message-perl
  libhttp-negotiate-perl libhyperscan5 libio-html-perl libio-socket-ssl-perl libjansson4 libltdl7 libluajit-5.1-2 libluajit-5.1-common liblwp-mediatypes-perl liblwp-protocol-https-perl libmailtools-perl
  libnet-http-perl libnet-smtp-ssl-perl libnet-ssleay-perl libnet1 libnetfilter-log1 libnetfilter-queue1 libnfnetlink0 libnspr4 libnss3 libpcap0.8 libprelude23 libpython-stdlib libpython2-stdlib
  libpython2.7-minimal libpython2.7-stdlib libtimedate-perl libtry-tiny-perl liburi-perl libwww-perl libwww-robotrules-perl libyaml-0-2 oinkmaster perl-openssl-defaults prelude-utils python python-minimal
  python-simplejson python2 python2-minimal python2.7 python2.7-minimal snort-rules-default suricata-oinkmaster
Suggested packages:
  libdigest-hmac-perl libgssapi-perl geoip-bin libcrypt-ssleay-perl libauthen-ntlm-perl python-doc python-tk python2-doc python2.7-doc binfmt-support snort | snort-pgsql | snort-mysql libtcmalloc-minimal4
The following NEW packages will be installed:
  geoip-database libauthen-sasl-perl libdata-dump-perl libencode-locale-perl libevent-2.1-6 libevent-core-2.1-6 libevent-pthreads-2.1-6 libfile-listing-perl libfont-afm-perl libgeoip1 libhiredis0.14
  libhtml-form-perl libhtml-format-perl libhtml-parser-perl libhtml-tagset-perl libhtml-tree-perl libhtp2 libhttp-cookies-perl libhttp-daemon-perl libhttp-date-perl libhttp-message-perl
  libhttp-negotiate-perl libhyperscan5 libio-html-perl libio-socket-ssl-perl libjansson4 libltdl7 libluajit-5.1-2 libluajit-5.1-common liblwp-mediatypes-perl liblwp-protocol-https-perl libmailtools-perl
  libnet-http-perl libnet-smtp-ssl-perl libnet-ssleay-perl libnet1 libnetfilter-log1 libnetfilter-queue1 libnfnetlink0 libnspr4 libnss3 libpcap0.8 libprelude23 libpython-stdlib libpython2-stdlib
  libpython2.7-minimal libpython2.7-stdlib libtimedate-perl libtry-tiny-perl liburi-perl libwww-perl libwww-robotrules-perl libyaml-0-2 oinkmaster perl-openssl-defaults prelude-utils python python-minimal
  python-simplejson python2 python2-minimal python2.7 python2.7-minimal snort-rules-default suricata suricata-oinkmaster
0 upgraded, 66 newly installed, 0 to remove and 42 not upgraded.
Need to get 16.8 MB of archives.
After this operation, 62.6 MB of additional disk space will be used.
Do you want to continue? [Y/n] suricata
Abort.
analyst@e980ac1fd1be:~$ sudo apt remove suricata 
Reading package lists... Done
Building dependency tree       
Reading state information... Done
Package 'suricata' is not installed, so not removed
0 upgraded, 0 newly installed, 0 to remove and 42 not upgraded.
analyst@e980ac1fd1be:~$ suricata
-bash: suricata: command not found
analyst@e980ac1fd1be:~$ sudo apt install tcpdump 
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following additional packages will be installed:
  libpcap0.8
Suggested packages:
  apparmor
The following NEW packages will be installed:
  libpcap0.8 tcpdump
0 upgraded, 2 newly installed, 0 to remove and 42 not upgraded.
Need to get 540 kB of archives.
After this operation, 1475 kB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://deb.debian.org/debian buster/main amd64 libpcap0.8 amd64 1.8.1-6+deb10u1 [140 kB]
Get:2 http://deb.debian.org/debian buster/main amd64 tcpdump amd64 4.9.3-1~deb10u2 [400 kB]
Fetched 540 kB in 0s (1999 kB/s)
debconf: delaying package configuration, since apt-utils is not installed
Selecting previously unselected package libpcap0.8:amd64.
(Reading database ... 22919 files and directories currently installed.)
Preparing to unpack .../libpcap0.8_1.8.1-6+deb10u1_amd64.deb ...
Unpacking libpcap0.8:amd64 (1.8.1-6+deb10u1) ...
Selecting previously unselected package tcpdump.
Preparing to unpack .../tcpdump_4.9.3-1~deb10u2_amd64.deb ...
Unpacking tcpdump (4.9.3-1~deb10u2) ...
Setting up libpcap0.8:amd64 (1.8.1-6+deb10u1) ...
Setting up tcpdump (4.9.3-1~deb10u2) ...
Processing triggers for man-db (2.8.5-2) ...
Processing triggers for libc-bin (2.28-10+deb10u2) ...
analyst@e980ac1fd1be:~$ apt list --installed 
Listing... Done
adduser/oldoldstable,now 3.118 all [installed,automatic]
apt/oldoldstable,oldoldstable-updates,now 1.8.2.3 amd64 [installed,automatic]
base-files/oldoldstable,now 10.3+deb10u13 amd64 [installed,automatic]
base-passwd/oldoldstable,now 3.5.46 amd64 [installed,automatic]
bash/oldoldstable,now 5.0-4 amd64 [installed,automatic]
binutils-common/oldoldstable,now 2.31.1-16 amd64 [installed,automatic]
binutils-x86-64-linux-gnu/oldoldstable,now 2.31.1-16 amd64 [installed,automatic]
binutils/oldoldstable,now 2.31.1-16 amd64 [installed,automatic]
bsdmainutils/oldoldstable,now 11.1.2+b1 amd64 [installed,automatic]
bsdutils/oldoldstable,now 1:2.33.1-0.1 amd64 [installed,automatic]
build-essential/oldoldstable,now 12.6 amd64 [installed,automatic]
bzip2/oldoldstable,now 1.0.6-9.2~deb10u2 amd64 [installed,automatic]
ca-certificates/oldoldstable,oldoldstable-updates,now 20200601~deb10u2 all [installed,automatic]
coreutils/oldoldstable,now 8.30-3 amd64 [installed,automatic]
cpp-8/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
cpp/oldoldstable,now 4:8.3.0-1 amd64 [installed,automatic]
dash/oldoldstable,now 0.5.10.2-5 amd64 [installed,automatic]
dbus/now 1.12.24-0+deb10u1 amd64 [installed,upgradable to: 1.12.28-0+deb10u1]
debconf/oldoldstable,now 1.5.71+deb10u1 all [installed,automatic]
debian-archive-keyring/oldoldstable,now 2019.1+deb10u1 all [installed,upgradable to: 2019.1+deb10u2]
debianutils/oldoldstable,now 4.8.6.1 amd64 [installed,automatic]
dh-python/oldoldstable,now 3.20190308 all [installed,automatic]
diffutils/oldoldstable,now 1:3.7-3 amd64 [installed,automatic]
dirmngr/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
dmsetup/oldoldstable,now 2:1.02.155-3 amd64 [installed,automatic]
dpkg-dev/oldoldstable,oldoldstable,now 1.19.8 all [installed,automatic]
dpkg/oldoldstable,oldoldstable,now 1.19.8 amd64 [installed,automatic]
e2fsprogs/oldoldstable,now 1.44.5-1+deb10u3 amd64 [installed,automatic]
fakeroot/oldoldstable,now 1.23-1 amd64 [installed,automatic]
fdisk/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
file/oldoldstable,now 1:5.35-4+deb10u2 amd64 [installed,automatic]
findutils/oldoldstable,now 4.6.0+git+20190209-2 amd64 [installed,automatic]
g++-8/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
g++/oldoldstable,now 4:8.3.0-1 amd64 [installed,automatic]
gcc-8-base/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
gcc-8/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
gcc/oldoldstable,now 4:8.3.0-1 amd64 [installed,automatic]
gir1.2-glib-2.0/oldoldstable,now 1.58.3-2 amd64 [installed,automatic]
gnupg-l10n/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 all [installed,automatic]
gnupg-utils/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gnupg/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 all [installed,automatic]
gpg-agent/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gpg-wks-client/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gpg-wks-server/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gpg/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gpgconf/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gpgsm/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gpgv/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
grep/oldoldstable,now 3.3-1 amd64 [installed,automatic]
groff-base/oldoldstable,now 1.22.4-3+deb10u1 amd64 [installed,automatic]
gzip/oldoldstable,oldoldstable,now 1.9-3+deb10u1 amd64 [installed,automatic]
hostname/oldoldstable,now 3.21 amd64 [installed,automatic]
info/oldoldstable,now 6.5.0.dfsg.1-4+b1 amd64 [installed]
init-system-helpers/oldoldstable,now 1.56+nmu1 all [installed,automatic]
install-info/oldoldstable,now 6.5.0.dfsg.1-4+b1 amd64 [installed,automatic]
iproute2/oldoldstable,now 4.20.0-2+deb10u1 amd64 [installed]
iputils-ping/oldoldstable,now 3:20180629-2+deb10u2 amd64 [installed]
krb5-locales/now 1.17-3+deb10u5 all [installed,upgradable to: 1.17-3+deb10u6]
libacl1/oldoldstable,now 2.2.53-4 amd64 [installed,automatic]
libalgorithm-diff-perl/oldoldstable,now 1.19.03-2 all [installed,automatic]
libalgorithm-diff-xs-perl/oldoldstable,now 0.04-5+b1 amd64 [installed,automatic]
libalgorithm-merge-perl/oldoldstable,now 0.08-3 all [installed,automatic]
libapparmor1/oldoldstable,now 2.13.2-10 amd64 [installed,automatic]
libapt-pkg5.0/oldoldstable,oldoldstable-updates,now 1.8.2.3 amd64 [installed,automatic]
libargon2-1/oldoldstable,now 0~20171227-0.2 amd64 [installed,automatic]
libasan5/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libassuan0/oldoldstable,now 2.5.2-1 amd64 [installed,automatic]
libatomic1/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libattr1/oldoldstable,now 1:2.4.48-4 amd64 [installed,automatic]
libaudit-common/oldoldstable,now 1:2.8.4-3 all [installed,automatic]
libaudit1/oldoldstable,now 1:2.8.4-3 amd64 [installed,automatic]
libbinutils/oldoldstable,now 2.31.1-16 amd64 [installed,automatic]
libblkid1/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
libbsd0/oldoldstable,now 0.9.1-2+deb10u1 amd64 [installed,automatic]
libbz2-1.0/oldoldstable,now 1.0.6-9.2~deb10u2 amd64 [installed,automatic]
libc-bin/oldoldstable,now 2.28-10+deb10u2 amd64 [installed,automatic]
libc-dev-bin/oldoldstable,now 2.28-10+deb10u2 amd64 [installed,automatic]
libc6-dev/oldoldstable,now 2.28-10+deb10u2 amd64 [installed,automatic]
libc6/oldoldstable,now 2.28-10+deb10u2 amd64 [installed,automatic]
libcap-ng0/oldoldstable,now 0.7.9-2 amd64 [installed,automatic]
libcap2-bin/oldoldstable,now 1:2.25-2 amd64 [installed,automatic]
libcap2/oldoldstable,now 1:2.25-2 amd64 [installed,automatic]
libcc1-0/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libcom-err2/oldoldstable,now 1.44.5-1+deb10u3 amd64 [installed,automatic]
libcryptsetup12/oldoldstable,now 2:2.1.0-5+deb10u2 amd64 [installed,automatic]
libdb5.3/oldoldstable,now 5.3.28+dfsg1-0.5 amd64 [installed,automatic]
libdbus-1-3/now 1.12.24-0+deb10u1 amd64 [installed,upgradable to: 1.12.28-0+deb10u1]
libdebconfclient0/oldoldstable,now 0.249 amd64 [installed,automatic]
libdevmapper1.02.1/oldoldstable,now 2:1.02.155-3 amd64 [installed,automatic]
libdpkg-perl/oldoldstable,oldoldstable,now 1.19.8 all [installed,automatic]
libedit2/oldoldstable,now 3.1-20181209-1 amd64 [installed,automatic]
libelf1/oldoldstable,now 0.176-1.1 amd64 [installed,upgradable to: 0.176-1.1+deb10u1]
libexpat1-dev/oldoldstable,now 2.2.6-2+deb10u6 amd64 [installed,automatic]
libexpat1/oldoldstable,now 2.2.6-2+deb10u6 amd64 [installed,automatic]
libext2fs2/oldoldstable,now 1.44.5-1+deb10u3 amd64 [installed,automatic]
libfakeroot/oldoldstable,now 1.23-1 amd64 [installed,automatic]
libfdisk1/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
libffi6/oldoldstable,now 3.2.1-9 amd64 [installed,automatic]
libfile-fcntllock-perl/oldoldstable,now 0.22-3+b5 amd64 [installed,automatic]
libgcc-8-dev/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libgcc1/oldoldstable,now 1:8.3.0-6 amd64 [installed,automatic]
libgcrypt20/oldoldstable,now 1.8.4-5+deb10u1 amd64 [installed,automatic]
libgdbm-compat4/oldoldstable,now 1.18.1-4 amd64 [installed,automatic]
libgdbm6/oldoldstable,now 1.18.1-4 amd64 [installed,automatic]
libgirepository-1.0-1/oldoldstable,now 1.58.3-2 amd64 [installed,automatic]
libglib2.0-0/now 2.58.3-2+deb10u4 amd64 [installed,upgradable to: 2.58.3-2+deb10u5]
libglib2.0-data/now 2.58.3-2+deb10u4 all [installed,upgradable to: 2.58.3-2+deb10u5]
libgmp10/oldoldstable,now 2:6.1.2+dfsg-4+deb10u1 amd64 [installed,automatic]
libgnutls30/now 3.6.7-4+deb10u10 amd64 [installed,upgradable to: 3.6.7-4+deb10u11]
libgomp1/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libgpg-error0/oldoldstable,now 1.35-1 amd64 [installed,automatic]
libgpm2/oldoldstable,now 1.20.7-5 amd64 [installed,automatic]
libgssapi-krb5-2/now 1.17-3+deb10u5 amd64 [installed,upgradable to: 1.17-3+deb10u6]
libhogweed4/oldoldstable,oldoldstable,now 3.4.1-1+deb10u1 amd64 [installed,automatic]
libicu63/oldoldstable,now 63.1-6+deb10u3 amd64 [installed,automatic]
libidn11/oldoldstable,now 1.33-2.2 amd64 [installed,automatic]
libidn2-0/oldoldstable,oldoldstable,now 2.0.5-1+deb10u1 amd64 [installed,automatic]
libip4tc0/oldoldstable,now 1.8.2-4 amd64 [installed,automatic]
libisl19/oldoldstable,now 0.20-2 amd64 [installed,automatic]
libitm1/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libjson-c3/oldoldstable,oldoldstable,now 0.12.1+ds-2+deb10u1 amd64 [installed,automatic]
libk5crypto3/now 1.17-3+deb10u5 amd64 [installed,upgradable to: 1.17-3+deb10u6]
libkeyutils1/oldoldstable,now 1.6-6 amd64 [installed,automatic]
libkmod2/oldoldstable,now 26-1 amd64 [installed,automatic]
libkrb5-3/now 1.17-3+deb10u5 amd64 [installed,upgradable to: 1.17-3+deb10u6]
libkrb5support0/now 1.17-3+deb10u5 amd64 [installed,upgradable to: 1.17-3+deb10u6]
libksba8/oldoldstable,now 1.3.5-2+deb10u2 amd64 [installed,automatic]
libldap-2.4-2/oldoldstable,oldoldstable,now 2.4.47+dfsg-3+deb10u7 amd64 [installed,automatic]
libldap-common/oldoldstable,oldoldstable,now 2.4.47+dfsg-3+deb10u7 all [installed,automatic]
liblocale-gettext-perl/oldoldstable,now 1.07-3+b4 amd64 [installed,automatic]
liblsan0/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
liblz4-1/oldoldstable,oldoldstable,now 1.8.3-1+deb10u1 amd64 [installed,automatic]
liblzma5/oldoldstable,oldoldstable,now 5.2.4-1+deb10u1 amd64 [installed,automatic]
libmagic-mgc/oldoldstable,now 1:5.35-4+deb10u2 amd64 [installed,automatic]
libmagic1/oldoldstable,now 1:5.35-4+deb10u2 amd64 [installed,automatic]
libmnl0/oldoldstable,now 1.0.4-2 amd64 [installed,automatic]
libmount1/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
libmpc3/oldoldstable,now 1.1.0-1 amd64 [installed,automatic]
libmpdec2/oldoldstable,now 2.4.2-2 amd64 [installed,automatic]
libmpfr6/oldoldstable,now 4.0.2-1 amd64 [installed,automatic]
libmpx2/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libncurses6/now 6.1+20181013-2+deb10u3 amd64 [installed,upgradable to: 6.1+20181013-2+deb10u5]
libncursesw6/now 6.1+20181013-2+deb10u3 amd64 [installed,upgradable to: 6.1+20181013-2+deb10u5]
libnettle6/oldoldstable,oldoldstable,now 3.4.1-1+deb10u1 amd64 [installed,automatic]
libnpth0/oldoldstable,now 1.6-1 amd64 [installed,automatic]
libnss-systemd/oldoldstable,now 241-7~deb10u8 amd64 [installed,upgradable to: 241-7~deb10u10]
libp11-kit0/oldoldstable,oldoldstable,now 0.23.15-2+deb10u1 amd64 [installed,automatic]
libpam-modules-bin/oldoldstable,now 1.3.1-5 amd64 [installed,automatic]
libpam-modules/oldoldstable,now 1.3.1-5 amd64 [installed,automatic]
libpam-runtime/oldoldstable,now 1.3.1-5 all [installed,automatic]
libpam-systemd/oldoldstable,now 241-7~deb10u8 amd64 [installed,upgradable to: 241-7~deb10u10]
libpam0g/oldoldstable,now 1.3.1-5 amd64 [installed,automatic]
libpcap0.8/oldoldstable,now 1.8.1-6+deb10u1 amd64 [installed,automatic]
libpcre2-8-0/oldoldstable,now 10.32-5 amd64 [installed,upgradable to: 10.32-5+deb10u1]
libpcre3/oldoldstable,now 2:8.39-12 amd64 [installed,automatic]
libperl5.28/oldoldstable,now 5.28.1-6+deb10u1 amd64 [installed,automatic]
libpipeline1/oldoldstable,now 1.5.1-2 amd64 [installed,automatic]
libprocps7/oldoldstable,now 2:3.3.15-2 amd64 [installed,automatic]
libpsl5/oldoldstable,now 0.20.2-2 amd64 [installed,automatic]
libpython3-dev/oldoldstable,now 3.7.3-1 amd64 [installed,automatic]
libpython3-stdlib/oldoldstable,now 3.7.3-1 amd64 [installed,automatic]
libpython3.7-dev/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
libpython3.7-minimal/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
libpython3.7-stdlib/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
libpython3.7/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
libquadmath0/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libreadline7/oldoldstable,now 7.0-5 amd64 [installed,automatic]
libsasl2-2/oldoldstable,oldoldstable,now 2.1.27+dfsg-1+deb10u2 amd64 [installed,automatic]
libsasl2-modules-db/oldoldstable,oldoldstable,now 2.1.27+dfsg-1+deb10u2 amd64 [installed,automatic]
libsasl2-modules/oldoldstable,oldoldstable,now 2.1.27+dfsg-1+deb10u2 amd64 [installed,automatic]
libseccomp2/oldoldstable,now 2.3.3-4 amd64 [installed,automatic]
libselinux1/oldoldstable,now 2.8-1+b1 amd64 [installed,automatic]
libsemanage-common/oldoldstable,now 2.8-2 all [installed,automatic]
libsemanage1/oldoldstable,now 2.8-2 amd64 [installed,automatic]
libsepol1/oldoldstable,now 2.8-1 amd64 [installed,automatic]
libsmartcols1/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
libsqlite3-0/oldoldstable,now 3.27.2-3+deb10u2 amd64 [installed,automatic]
libss2/oldoldstable,now 1.44.5-1+deb10u3 amd64 [installed,automatic]
libssl1.1/now 1.1.1n-0+deb10u4 amd64 [installed,upgradable to: 1.1.1n-0+deb10u6]
libstdc++-8-dev/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libstdc++6/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libsystemd0/oldoldstable,now 241-7~deb10u8 amd64 [installed,upgradable to: 241-7~deb10u10]
libtasn1-6/oldoldstable,now 4.13-3+deb10u1 amd64 [installed,automatic]
libtinfo6/now 6.1+20181013-2+deb10u3 amd64 [installed,upgradable to: 6.1+20181013-2+deb10u5]
libtsan0/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libubsan1/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libuchardet0/oldoldstable,now 0.0.6-3 amd64 [installed,automatic]
libudev1/oldoldstable,now 241-7~deb10u8 amd64 [installed,upgradable to: 241-7~deb10u10]
libunistring2/oldoldstable,now 0.9.10-1 amd64 [installed,automatic]
libuuid1/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
libwrap0/oldoldstable,now 7.6.q-28 amd64 [installed,automatic]
libx11-6/oldoldstable,now 2:1.6.7-1+deb10u2 amd64 [installed,upgradable to: 2:1.6.7-1+deb10u4]
libx11-data/oldoldstable,now 2:1.6.7-1+deb10u2 all [installed,upgradable to: 2:1.6.7-1+deb10u4]
libxau6/oldoldstable,now 1:1.0.8-1+b2 amd64 [installed,automatic]
libxcb1/oldoldstable,now 1.13.1-2 amd64 [installed,automatic]
libxdmcp6/oldoldstable,now 1:1.1.2-3 amd64 [installed,automatic]
libxext6/oldoldstable,now 2:1.3.3-1+b2 amd64 [installed,automatic]
libxml2/now 2.9.4+dfsg1-7+deb10u5 amd64 [installed,upgradable to: 2.9.4+dfsg1-7+deb10u6]
libxmuu1/oldoldstable,now 2:1.1.2-2+b3 amd64 [installed,automatic]
libxtables12/oldoldstable,now 1.8.2-4 amd64 [installed,automatic]
libzstd1/oldoldstable,oldoldstable,now 1.3.8+dfsg-3+deb10u2 amd64 [installed,automatic]
linux-libc-dev/now 4.19.269-1 amd64 [installed,upgradable to: 4.19.289-2]
login/oldoldstable,now 1:4.5-1.1 amd64 [installed,automatic]
lsb-base/oldoldstable,now 10.2019051400 all [installed,automatic]
make/oldoldstable,now 4.2.1-1.2 amd64 [installed,automatic]
man-db/oldoldstable,now 2.8.5-2 amd64 [installed]
manpages-dev/oldoldstable,now 4.16-2 all [installed,automatic]
manpages/oldoldstable,now 4.16-2 all [installed,automatic]
mawk/oldoldstable,now 1.3.3-17+b3 amd64 [installed,automatic]
mime-support/oldoldstable,now 3.62 all [installed,automatic]
mount/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
nano/oldoldstable,now 3.2-3 amd64 [installed]
ncurses-base/now 6.1+20181013-2+deb10u3 all [installed,upgradable to: 6.1+20181013-2+deb10u5]
ncurses-bin/now 6.1+20181013-2+deb10u3 amd64 [installed,upgradable to: 6.1+20181013-2+deb10u5]
ncurses-term/now 6.1+20181013-2+deb10u3 all [installed,upgradable to: 6.1+20181013-2+deb10u5]
netbase/oldoldstable,now 5.6 all [installed,automatic]
openssh-client/oldoldstable,now 1:7.9p1-10+deb10u2 amd64 [installed,upgradable to: 1:7.9p1-10+deb10u3]
openssh-server/oldoldstable,now 1:7.9p1-10+deb10u2 amd64 [installed,upgradable to: 1:7.9p1-10+deb10u3]
openssh-sftp-server/oldoldstable,now 1:7.9p1-10+deb10u2 amd64 [installed,upgradable to: 1:7.9p1-10+deb10u3]
openssl/now 1.1.1n-0+deb10u4 amd64 [installed,upgradable to: 1.1.1n-0+deb10u6]
passwd/oldoldstable,now 1:4.5-1.1 amd64 [installed,automatic]
patch/oldoldstable,oldoldstable,now 2.7.6-3+deb10u1 amd64 [installed,automatic]
perl-base/oldoldstable,now 5.28.1-6+deb10u1 amd64 [installed,automatic]
perl-modules-5.28/oldoldstable,now 5.28.1-6+deb10u1 all [installed,automatic]
perl/oldoldstable,now 5.28.1-6+deb10u1 amd64 [installed,automatic]
pinentry-curses/oldoldstable,now 1.1.0-2 amd64 [installed,automatic]
procps/oldoldstable,now 2:3.3.15-2 amd64 [installed,automatic]
psmisc/oldoldstable,now 23.2-1+deb10u1 amd64 [installed,automatic]
publicsuffix/oldoldstable,now 20220811.1734-0+deb10u1 all [installed,automatic]
python-pip-whl/oldoldstable,now 18.1-5 all [installed,automatic]
python3-asn1crypto/oldoldstable,now 0.24.0-1 all [installed,automatic]
python3-cffi-backend/oldoldstable,now 1.12.2-1 amd64 [installed,automatic]
python3-crypto/oldoldstable,now 2.6.1-9+b1 amd64 [installed,automatic]
python3-cryptography/oldoldstable,now 2.6.1-3+deb10u4 amd64 [installed,automatic]
python3-dbus/oldoldstable,now 1.2.8-3 amd64 [installed,automatic]
python3-dev/oldoldstable,now 3.7.3-1 amd64 [installed,automatic]
python3-distutils/oldoldstable,now 3.7.3-1 all [installed,automatic]
python3-entrypoints/oldoldstable,now 0.3-1 all [installed,automatic]
python3-gi/oldoldstable,now 3.30.4-1 amd64 [installed,automatic]
python3-keyring/oldoldstable,now 17.1.1-1 all [installed,automatic]
python3-keyrings.alt/oldoldstable,now 3.1.1-1 all [installed,automatic]
python3-lib2to3/oldoldstable,now 3.7.3-1 all [installed,automatic]
python3-minimal/oldoldstable,now 3.7.3-1 amd64 [installed,automatic]
python3-pip/oldoldstable,now 18.1-5 all [installed]
python3-pkg-resources/oldoldstable,now 40.8.0-1 all [installed,automatic]
python3-secretstorage/oldoldstable,now 2.3.1-2 all [installed,automatic]
python3-setuptools/oldoldstable,now 40.8.0-1 all [installed,automatic]
python3-six/oldoldstable,now 1.12.0-1 all [installed,automatic]
python3-wheel/oldoldstable,now 0.32.3-2 all [installed,automatic]
python3-xdg/oldoldstable,now 0.25-5 all [installed,automatic]
python3.7-dev/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
python3.7-minimal/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
python3.7/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
python3/oldoldstable,now 3.7.3-1 amd64 [installed]
readline-common/oldoldstable,now 7.0-5 all [installed,automatic]
sed/oldoldstable,now 4.7-1 amd64 [installed,automatic]
sensible-utils/oldoldstable,now 0.0.12 all [installed,automatic]
shared-mime-info/oldoldstable,now 1.10-1 amd64 [installed,automatic]
sudo/oldoldstable,now 1.8.27-1+deb10u5 amd64 [installed]
systemd-sysv/oldoldstable,now 241-7~deb10u8 amd64 [installed,upgradable to: 241-7~deb10u10]
systemd/oldoldstable,now 241-7~deb10u8 amd64 [installed,upgradable to: 241-7~deb10u10]
sysvinit-utils/oldoldstable,now 2.93-8 amd64 [installed,automatic]
tar/oldoldstable,now 1.30+dfsg-6 amd64 [installed,automatic]
tcpdump/oldoldstable,now 4.9.3-1~deb10u2 amd64 [installed]
tree/oldoldstable,now 1.8.0-1 amd64 [installed]
tzdata/now 2021a-0+deb10u8 all [installed,upgradable to: 2021a-0+deb10u12]
ucf/oldoldstable,now 3.0038+nmu1 all [installed,automatic]
util-linux/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
wget/oldoldstable,now 1.20.1-1.1 amd64 [installed]
xauth/oldoldstable,now 1:1.0.10-1 amd64 [installed,automatic]
xdg-user-dirs/oldoldstable,now 0.17-2 amd64 [installed,automatic]
xz-utils/oldoldstable,oldoldstable,now 5.2.4-1+deb10u1 amd64 [installed,automatic]
zlib1g/oldoldstable,now 1:1.2.11.dfsg-1+deb10u2 amd64 [installed,automatic]
analyst@e980ac1fd1be:~$ sudo apt install suricata 
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following additional packages will be installed:
  geoip-database libauthen-sasl-perl libdata-dump-perl libencode-locale-perl libevent-2.1-6 libevent-core-2.1-6 libevent-pthreads-2.1-6 libfile-listing-perl libfont-afm-perl libgeoip1 libhiredis0.14
  libhtml-form-perl libhtml-format-perl libhtml-parser-perl libhtml-tagset-perl libhtml-tree-perl libhtp2 libhttp-cookies-perl libhttp-daemon-perl libhttp-date-perl libhttp-message-perl
  libhttp-negotiate-perl libhyperscan5 libio-html-perl libio-socket-ssl-perl libjansson4 libltdl7 libluajit-5.1-2 libluajit-5.1-common liblwp-mediatypes-perl liblwp-protocol-https-perl libmailtools-perl
  libnet-http-perl libnet-smtp-ssl-perl libnet-ssleay-perl libnet1 libnetfilter-log1 libnetfilter-queue1 libnfnetlink0 libnspr4 libnss3 libprelude23 libpython-stdlib libpython2-stdlib libpython2.7-minimal
  libpython2.7-stdlib libtimedate-perl libtry-tiny-perl liburi-perl libwww-perl libwww-robotrules-perl libyaml-0-2 oinkmaster perl-openssl-defaults prelude-utils python python-minimal python-simplejson
  python2 python2-minimal python2.7 python2.7-minimal snort-rules-default suricata-oinkmaster
Suggested packages:
  libdigest-hmac-perl libgssapi-perl geoip-bin libcrypt-ssleay-perl libauthen-ntlm-perl python-doc python-tk python2-doc python2.7-doc binfmt-support snort | snort-pgsql | snort-mysql libtcmalloc-minimal4
The following NEW packages will be installed:
  geoip-database libauthen-sasl-perl libdata-dump-perl libencode-locale-perl libevent-2.1-6 libevent-core-2.1-6 libevent-pthreads-2.1-6 libfile-listing-perl libfont-afm-perl libgeoip1 libhiredis0.14
  libhtml-form-perl libhtml-format-perl libhtml-parser-perl libhtml-tagset-perl libhtml-tree-perl libhtp2 libhttp-cookies-perl libhttp-daemon-perl libhttp-date-perl libhttp-message-perl
  libhttp-negotiate-perl libhyperscan5 libio-html-perl libio-socket-ssl-perl libjansson4 libltdl7 libluajit-5.1-2 libluajit-5.1-common liblwp-mediatypes-perl liblwp-protocol-https-perl libmailtools-perl
  libnet-http-perl libnet-smtp-ssl-perl libnet-ssleay-perl libnet1 libnetfilter-log1 libnetfilter-queue1 libnfnetlink0 libnspr4 libnss3 libprelude23 libpython-stdlib libpython2-stdlib libpython2.7-minimal
  libpython2.7-stdlib libtimedate-perl libtry-tiny-perl liburi-perl libwww-perl libwww-robotrules-perl libyaml-0-2 oinkmaster perl-openssl-defaults prelude-utils python python-minimal python-simplejson
  python2 python2-minimal python2.7 python2.7-minimal snort-rules-default suricata suricata-oinkmaster
0 upgraded, 65 newly installed, 0 to remove and 42 not upgraded.
Need to get 16.6 MB of archives.
After this operation, 62.2 MB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://deb.debian.org/debian-security buster/updates/main amd64 libpython2.7-minimal amd64 2.7.16-2+deb10u3 [397 kB]
Get:2 http://deb.debian.org/debian-security buster/updates/main amd64 python2.7-minimal amd64 2.7.16-2+deb10u3 [1362 kB]
Get:3 http://deb.debian.org/debian buster/main amd64 python2-minimal amd64 2.7.16-1 [41.4 kB]
Get:4 http://deb.debian.org/debian buster/main amd64 python-minimal amd64 2.7.16-1 [21.0 kB]
Get:5 http://deb.debian.org/debian-security buster/updates/main amd64 libpython2.7-stdlib amd64 2.7.16-2+deb10u3 [1910 kB]
Get:6 http://deb.debian.org/debian-security buster/updates/main amd64 python2.7 amd64 2.7.16-2+deb10u3 [306 kB]
Get:7 http://deb.debian.org/debian buster/main amd64 libpython2-stdlib amd64 2.7.16-1 [20.8 kB]
Get:8 http://deb.debian.org/debian buster/main amd64 libpython-stdlib amd64 2.7.16-1 [20.8 kB]
Get:9 http://deb.debian.org/debian buster/main amd64 python2 amd64 2.7.16-1 [41.6 kB]
Get:10 http://deb.debian.org/debian buster/main amd64 python amd64 2.7.16-1 [22.8 kB]
Get:11 http://deb.debian.org/debian buster/main amd64 libhyperscan5 amd64 5.1.0-1 [2349 kB]
Get:12 http://deb.debian.org/debian buster/main amd64 python-simplejson amd64 3.16.0-1 [72.6 kB]
Get:13 http://deb.debian.org/debian buster/main amd64 libevent-2.1-6 amd64 2.1.8-stable-4 [177 kB]
Get:14 http://deb.debian.org/debian buster/main amd64 libevent-core-2.1-6 amd64 2.1.8-stable-4 [129 kB]
Get:15 http://deb.debian.org/debian buster/main amd64 libevent-pthreads-2.1-6 amd64 2.1.8-stable-4 [47.9 kB]
Get:16 http://deb.debian.org/debian buster/main amd64 libgeoip1 amd64 1.6.12-1 [93.1 kB]
Get:17 http://deb.debian.org/debian buster/main amd64 libhiredis0.14 amd64 0.14.0-3 [33.8 kB]
Get:18 http://deb.debian.org/debian buster/main amd64 libhtp2 amd64 1:0.5.30-1 [55.6 kB]
Get:19 http://deb.debian.org/debian buster/main amd64 libjansson4 amd64 2.12-1 [38.0 kB]
Get:20 http://deb.debian.org/debian buster/main amd64 libltdl7 amd64 2.4.6-9 [390 kB]
Get:21 http://deb.debian.org/debian buster/main amd64 libluajit-5.1-common all 2.1.0~beta3+dfsg-5.1 [46.7 kB]
Get:22 http://deb.debian.org/debian buster/main amd64 libluajit-5.1-2 amd64 2.1.0~beta3+dfsg-5.1 [230 kB]
Get:23 http://deb.debian.org/debian buster/main amd64 libnet1 amd64 1.1.6+dfsg-3.1 [60.4 kB]
Get:24 http://deb.debian.org/debian buster/main amd64 libnfnetlink0 amd64 1.0.1-3+b1 [13.9 kB]
Get:25 http://deb.debian.org/debian buster/main amd64 libnetfilter-log1 amd64 1.0.1-1.1+b1 [9782 B]
Get:26 http://deb.debian.org/debian buster/main amd64 libnetfilter-queue1 amd64 1.0.3-1 [12.5 kB]
Get:27 http://deb.debian.org/debian buster/main amd64 libnspr4 amd64 2:4.20-1 [112 kB]
Get:28 http://deb.debian.org/debian-security buster/updates/main amd64 libnss3 amd64 2:3.42.1-1+deb10u7 [1246 kB]
Get:29 http://deb.debian.org/debian buster/main amd64 libprelude23 amd64 4.1.0-4.2 [612 kB]
Get:30 http://deb.debian.org/debian buster/main amd64 libyaml-0-2 amd64 0.2.1-1 [47.2 kB]
Get:31 http://deb.debian.org/debian buster/main amd64 suricata amd64 1:4.1.2-2+deb10u1 [1660 kB]
Get:32 http://deb.debian.org/debian buster/main amd64 geoip-database all 20181108-1 [2449 kB]
Get:33 http://deb.debian.org/debian buster/main amd64 libauthen-sasl-perl all 2.1600-1 [50.8 kB]
Get:34 http://deb.debian.org/debian buster/main amd64 libdata-dump-perl all 1.23-1 [29.5 kB]
Get:35 http://deb.debian.org/debian buster/main amd64 libencode-locale-perl all 1.05-1 [13.7 kB]
Get:36 http://deb.debian.org/debian buster/main amd64 libtimedate-perl all 2.3000-2+deb10u1 [38.1 kB]
Get:37 http://deb.debian.org/debian buster/main amd64 libhttp-date-perl all 6.02-1 [10.7 kB]
Get:38 http://deb.debian.org/debian buster/main amd64 libfile-listing-perl all 6.04-1 [10.3 kB]
Get:39 http://deb.debian.org/debian buster/main amd64 libfont-afm-perl all 1.20-2 [13.6 kB]
Get:40 http://deb.debian.org/debian buster/main amd64 libhtml-tagset-perl all 3.20-3 [12.7 kB]
Get:41 http://deb.debian.org/debian buster/main amd64 liburi-perl all 1.76-1 [89.9 kB]
Get:42 http://deb.debian.org/debian buster/main amd64 libhtml-parser-perl amd64 3.72-3+b3 [105 kB]
Get:43 http://deb.debian.org/debian buster/main amd64 libio-html-perl all 1.001-1 [17.6 kB]
Get:44 http://deb.debian.org/debian buster/main amd64 liblwp-mediatypes-perl all 6.02-1 [22.1 kB]
Get:45 http://deb.debian.org/debian buster/main amd64 libhttp-message-perl all 6.18-1 [77.8 kB]
Get:46 http://deb.debian.org/debian buster/main amd64 libhtml-form-perl all 6.03-1 [23.9 kB]
Get:47 http://deb.debian.org/debian buster/main amd64 libhtml-tree-perl all 5.07-2 [213 kB]
Get:48 http://deb.debian.org/debian buster/main amd64 libhtml-format-perl all 2.12-1 [43.5 kB]
Get:49 http://deb.debian.org/debian buster/main amd64 libhttp-cookies-perl all 6.04-1 [17.8 kB]
Get:50 http://deb.debian.org/debian-security buster/updates/main amd64 libhttp-daemon-perl all 6.01-3+deb10u1 [17.1 kB]
Get:51 http://deb.debian.org/debian buster/main amd64 libhttp-negotiate-perl all 6.01-1 [12.8 kB]
Get:52 http://deb.debian.org/debian buster/main amd64 perl-openssl-defaults amd64 3 [6782 B]
Get:53 http://deb.debian.org/debian buster/main amd64 libnet-ssleay-perl amd64 1.85-2+deb10u1 [308 kB]
Get:54 http://deb.debian.org/debian buster/main amd64 libio-socket-ssl-perl all 2.060-3 [207 kB]
Get:55 http://deb.debian.org/debian buster/main amd64 libnet-http-perl all 6.18-1 [24.5 kB]
Get:56 http://deb.debian.org/debian buster/main amd64 libtry-tiny-perl all 0.30-1 [23.3 kB]
Get:57 http://deb.debian.org/debian buster/main amd64 libwww-robotrules-perl all 6.02-1 [12.9 kB]
Get:58 http://deb.debian.org/debian buster/main amd64 libwww-perl all 6.36-2 [188 kB]
Get:59 http://deb.debian.org/debian buster/main amd64 liblwp-protocol-https-perl all 6.07-2 [9242 B]
Get:60 http://deb.debian.org/debian buster/main amd64 libnet-smtp-ssl-perl all 1.04-1 [6184 B]
Get:61 http://deb.debian.org/debian buster/main amd64 libmailtools-perl all 2.18-1 [88.5 kB]
Get:62 http://deb.debian.org/debian buster/main amd64 oinkmaster all 2.0-4 [90.6 kB]
Get:63 http://deb.debian.org/debian buster/main amd64 prelude-utils amd64 4.1.0-4.2 [411 kB]
Get:64 http://deb.debian.org/debian-security buster/updates/main amd64 snort-rules-default all 2.9.20-0+deb10u1 [374 kB]
Get:65 http://deb.debian.org/debian buster/main amd64 suricata-oinkmaster all 1:4.1.2-2+deb10u1 [38.5 kB]
Fetched 16.6 MB in 2s (10.9 MB/s)           
debconf: delaying package configuration, since apt-utils is not installed
Selecting previously unselected package libpython2.7-minimal:amd64.
(Reading database ... 22943 files and directories currently installed.)
Preparing to unpack .../0-libpython2.7-minimal_2.7.16-2+deb10u3_amd64.deb ...
Unpacking libpython2.7-minimal:amd64 (2.7.16-2+deb10u3) ...
Selecting previously unselected package python2.7-minimal.
Preparing to unpack .../1-python2.7-minimal_2.7.16-2+deb10u3_amd64.deb ...
Unpacking python2.7-minimal (2.7.16-2+deb10u3) ...
Selecting previously unselected package python2-minimal.
Preparing to unpack .../2-python2-minimal_2.7.16-1_amd64.deb ...
Unpacking python2-minimal (2.7.16-1) ...
Selecting previously unselected package python-minimal.
Preparing to unpack .../3-python-minimal_2.7.16-1_amd64.deb ...
Unpacking python-minimal (2.7.16-1) ...
Selecting previously unselected package libpython2.7-stdlib:amd64.
Preparing to unpack .../4-libpython2.7-stdlib_2.7.16-2+deb10u3_amd64.deb ...
Unpacking libpython2.7-stdlib:amd64 (2.7.16-2+deb10u3) ...
Selecting previously unselected package python2.7.
Preparing to unpack .../5-python2.7_2.7.16-2+deb10u3_amd64.deb ...
Unpacking python2.7 (2.7.16-2+deb10u3) ...
Selecting previously unselected package libpython2-stdlib:amd64.
Preparing to unpack .../6-libpython2-stdlib_2.7.16-1_amd64.deb ...
Unpacking libpython2-stdlib:amd64 (2.7.16-1) ...
Selecting previously unselected package libpython-stdlib:amd64.
Preparing to unpack .../7-libpython-stdlib_2.7.16-1_amd64.deb ...
Unpacking libpython-stdlib:amd64 (2.7.16-1) ...
Setting up libpython2.7-minimal:amd64 (2.7.16-2+deb10u3) ...
Setting up python2.7-minimal (2.7.16-2+deb10u3) ...
Linking and byte-compiling packages for runtime python2.7...
Setting up python2-minimal (2.7.16-1) ...
Selecting previously unselected package python2.
(Reading database ... 23702 files and directories currently installed.)
Preparing to unpack .../python2_2.7.16-1_amd64.deb ...
Unpacking python2 (2.7.16-1) ...
Setting up python-minimal (2.7.16-1) ...
Selecting previously unselected package python.
(Reading database ... 23730 files and directories currently installed.)
Preparing to unpack .../00-python_2.7.16-1_amd64.deb ...
Unpacking python (2.7.16-1) ...
Selecting previously unselected package libhyperscan5.
Preparing to unpack .../01-libhyperscan5_5.1.0-1_amd64.deb ...
Unpacking libhyperscan5 (5.1.0-1) ...
Selecting previously unselected package python-simplejson.
Preparing to unpack .../02-python-simplejson_3.16.0-1_amd64.deb ...
Unpacking python-simplejson (3.16.0-1) ...
Selecting previously unselected package libevent-2.1-6:amd64.
Preparing to unpack .../03-libevent-2.1-6_2.1.8-stable-4_amd64.deb ...
Unpacking libevent-2.1-6:amd64 (2.1.8-stable-4) ...
Selecting previously unselected package libevent-core-2.1-6:amd64.
Preparing to unpack .../04-libevent-core-2.1-6_2.1.8-stable-4_amd64.deb ...
Unpacking libevent-core-2.1-6:amd64 (2.1.8-stable-4) ...
Selecting previously unselected package libevent-pthreads-2.1-6:amd64.
Preparing to unpack .../05-libevent-pthreads-2.1-6_2.1.8-stable-4_amd64.deb ...
Unpacking libevent-pthreads-2.1-6:amd64 (2.1.8-stable-4) ...
Selecting previously unselected package libgeoip1:amd64.
Preparing to unpack .../06-libgeoip1_1.6.12-1_amd64.deb ...
Unpacking libgeoip1:amd64 (1.6.12-1) ...
Selecting previously unselected package libhiredis0.14:amd64.
Preparing to unpack .../07-libhiredis0.14_0.14.0-3_amd64.deb ...
Unpacking libhiredis0.14:amd64 (0.14.0-3) ...
Selecting previously unselected package libhtp2.
Preparing to unpack .../08-libhtp2_1%3a0.5.30-1_amd64.deb ...
Unpacking libhtp2 (1:0.5.30-1) ...
Selecting previously unselected package libjansson4:amd64.
Preparing to unpack .../09-libjansson4_2.12-1_amd64.deb ...
Unpacking libjansson4:amd64 (2.12-1) ...
Selecting previously unselected package libltdl7:amd64.
Preparing to unpack .../10-libltdl7_2.4.6-9_amd64.deb ...
Unpacking libltdl7:amd64 (2.4.6-9) ...
Selecting previously unselected package libluajit-5.1-common.
Preparing to unpack .../11-libluajit-5.1-common_2.1.0~beta3+dfsg-5.1_all.deb ...
Unpacking libluajit-5.1-common (2.1.0~beta3+dfsg-5.1) ...
Selecting previously unselected package libluajit-5.1-2:amd64.
Preparing to unpack .../12-libluajit-5.1-2_2.1.0~beta3+dfsg-5.1_amd64.deb ...
Unpacking libluajit-5.1-2:amd64 (2.1.0~beta3+dfsg-5.1) ...
Selecting previously unselected package libnet1:amd64.
Preparing to unpack .../13-libnet1_1.1.6+dfsg-3.1_amd64.deb ...
Unpacking libnet1:amd64 (1.1.6+dfsg-3.1) ...
Selecting previously unselected package libnfnetlink0:amd64.
Preparing to unpack .../14-libnfnetlink0_1.0.1-3+b1_amd64.deb ...
Unpacking libnfnetlink0:amd64 (1.0.1-3+b1) ...
Selecting previously unselected package libnetfilter-log1:amd64.
Preparing to unpack .../15-libnetfilter-log1_1.0.1-1.1+b1_amd64.deb ...
Unpacking libnetfilter-log1:amd64 (1.0.1-1.1+b1) ...
Selecting previously unselected package libnetfilter-queue1.
Preparing to unpack .../16-libnetfilter-queue1_1.0.3-1_amd64.deb ...
Unpacking libnetfilter-queue1 (1.0.3-1) ...
Selecting previously unselected package libnspr4:amd64.
Preparing to unpack .../17-libnspr4_2%3a4.20-1_amd64.deb ...
Unpacking libnspr4:amd64 (2:4.20-1) ...
Selecting previously unselected package libnss3:amd64.
Preparing to unpack .../18-libnss3_2%3a3.42.1-1+deb10u7_amd64.deb ...
Unpacking libnss3:amd64 (2:3.42.1-1+deb10u7) ...
Selecting previously unselected package libprelude23:amd64.
Preparing to unpack .../19-libprelude23_4.1.0-4.2_amd64.deb ...
Unpacking libprelude23:amd64 (4.1.0-4.2) ...
Selecting previously unselected package libyaml-0-2:amd64.
Preparing to unpack .../20-libyaml-0-2_0.2.1-1_amd64.deb ...
Unpacking libyaml-0-2:amd64 (0.2.1-1) ...
Selecting previously unselected package suricata.
Preparing to unpack .../21-suricata_1%3a4.1.2-2+deb10u1_amd64.deb ...
Unpacking suricata (1:4.1.2-2+deb10u1) ...
Selecting previously unselected package geoip-database.
Preparing to unpack .../22-geoip-database_20181108-1_all.deb ...
Unpacking geoip-database (20181108-1) ...
Selecting previously unselected package libauthen-sasl-perl.
Preparing to unpack .../23-libauthen-sasl-perl_2.1600-1_all.deb ...
Unpacking libauthen-sasl-perl (2.1600-1) ...
Selecting previously unselected package libdata-dump-perl.
Preparing to unpack .../24-libdata-dump-perl_1.23-1_all.deb ...
Unpacking libdata-dump-perl (1.23-1) ...
Selecting previously unselected package libencode-locale-perl.
Preparing to unpack .../25-libencode-locale-perl_1.05-1_all.deb ...
Unpacking libencode-locale-perl (1.05-1) ...
Selecting previously unselected package libtimedate-perl.
Preparing to unpack .../26-libtimedate-perl_2.3000-2+deb10u1_all.deb ...
Unpacking libtimedate-perl (2.3000-2+deb10u1) ...
Selecting previously unselected package libhttp-date-perl.
Preparing to unpack .../27-libhttp-date-perl_6.02-1_all.deb ...
Unpacking libhttp-date-perl (6.02-1) ...
Selecting previously unselected package libfile-listing-perl.
Preparing to unpack .../28-libfile-listing-perl_6.04-1_all.deb ...
Unpacking libfile-listing-perl (6.04-1) ...
Selecting previously unselected package libfont-afm-perl.
Preparing to unpack .../29-libfont-afm-perl_1.20-2_all.deb ...
Unpacking libfont-afm-perl (1.20-2) ...
Selecting previously unselected package libhtml-tagset-perl.
Preparing to unpack .../30-libhtml-tagset-perl_3.20-3_all.deb ...
Unpacking libhtml-tagset-perl (3.20-3) ...
Selecting previously unselected package liburi-perl.
Preparing to unpack .../31-liburi-perl_1.76-1_all.deb ...
Unpacking liburi-perl (1.76-1) ...
Selecting previously unselected package libhtml-parser-perl.
Preparing to unpack .../32-libhtml-parser-perl_3.72-3+b3_amd64.deb ...
Unpacking libhtml-parser-perl (3.72-3+b3) ...
Selecting previously unselected package libio-html-perl.
Preparing to unpack .../33-libio-html-perl_1.001-1_all.deb ...
Unpacking libio-html-perl (1.001-1) ...
Selecting previously unselected package liblwp-mediatypes-perl.
Preparing to unpack .../34-liblwp-mediatypes-perl_6.02-1_all.deb ...
Unpacking liblwp-mediatypes-perl (6.02-1) ...
Selecting previously unselected package libhttp-message-perl.
Preparing to unpack .../35-libhttp-message-perl_6.18-1_all.deb ...
Unpacking libhttp-message-perl (6.18-1) ...
Selecting previously unselected package libhtml-form-perl.
Preparing to unpack .../36-libhtml-form-perl_6.03-1_all.deb ...
Unpacking libhtml-form-perl (6.03-1) ...
Selecting previously unselected package libhtml-tree-perl.
Preparing to unpack .../37-libhtml-tree-perl_5.07-2_all.deb ...
Unpacking libhtml-tree-perl (5.07-2) ...
Selecting previously unselected package libhtml-format-perl.
Preparing to unpack .../38-libhtml-format-perl_2.12-1_all.deb ...
Unpacking libhtml-format-perl (2.12-1) ...
Selecting previously unselected package libhttp-cookies-perl.
Preparing to unpack .../39-libhttp-cookies-perl_6.04-1_all.deb ...
Unpacking libhttp-cookies-perl (6.04-1) ...
Selecting previously unselected package libhttp-daemon-perl.
Preparing to unpack .../40-libhttp-daemon-perl_6.01-3+deb10u1_all.deb ...
Unpacking libhttp-daemon-perl (6.01-3+deb10u1) ...
Selecting previously unselected package libhttp-negotiate-perl.
Preparing to unpack .../41-libhttp-negotiate-perl_6.01-1_all.deb ...
Unpacking libhttp-negotiate-perl (6.01-1) ...
Selecting previously unselected package perl-openssl-defaults:amd64.
Preparing to unpack .../42-perl-openssl-defaults_3_amd64.deb ...
Unpacking perl-openssl-defaults:amd64 (3) ...
Selecting previously unselected package libnet-ssleay-perl.
Preparing to unpack .../43-libnet-ssleay-perl_1.85-2+deb10u1_amd64.deb ...
Unpacking libnet-ssleay-perl (1.85-2+deb10u1) ...
Selecting previously unselected package libio-socket-ssl-perl.
Preparing to unpack .../44-libio-socket-ssl-perl_2.060-3_all.deb ...
Unpacking libio-socket-ssl-perl (2.060-3) ...
Selecting previously unselected package libnet-http-perl.
Preparing to unpack .../45-libnet-http-perl_6.18-1_all.deb ...
Unpacking libnet-http-perl (6.18-1) ...
Selecting previously unselected package libtry-tiny-perl.
Preparing to unpack .../46-libtry-tiny-perl_0.30-1_all.deb ...
Unpacking libtry-tiny-perl (0.30-1) ...
Selecting previously unselected package libwww-robotrules-perl.
Preparing to unpack .../47-libwww-robotrules-perl_6.02-1_all.deb ...
Unpacking libwww-robotrules-perl (6.02-1) ...
Selecting previously unselected package libwww-perl.
Preparing to unpack .../48-libwww-perl_6.36-2_all.deb ...
Unpacking libwww-perl (6.36-2) ...
Selecting previously unselected package liblwp-protocol-https-perl.
Preparing to unpack .../49-liblwp-protocol-https-perl_6.07-2_all.deb ...
Unpacking liblwp-protocol-https-perl (6.07-2) ...
Selecting previously unselected package libnet-smtp-ssl-perl.
Preparing to unpack .../50-libnet-smtp-ssl-perl_1.04-1_all.deb ...
Unpacking libnet-smtp-ssl-perl (1.04-1) ...
Selecting previously unselected package libmailtools-perl.
Preparing to unpack .../51-libmailtools-perl_2.18-1_all.deb ...
Unpacking libmailtools-perl (2.18-1) ...
Selecting previously unselected package oinkmaster.
Preparing to unpack .../52-oinkmaster_2.0-4_all.deb ...
Unpacking oinkmaster (2.0-4) ...
Selecting previously unselected package prelude-utils.
Preparing to unpack .../53-prelude-utils_4.1.0-4.2_amd64.deb ...
Unpacking prelude-utils (4.1.0-4.2) ...
Selecting previously unselected package snort-rules-default.
Preparing to unpack .../54-snort-rules-default_2.9.20-0+deb10u1_all.deb ...
Unpacking snort-rules-default (2.9.20-0+deb10u1) ...
Selecting previously unselected package suricata-oinkmaster.
Preparing to unpack .../55-suricata-oinkmaster_1%3a4.1.2-2+deb10u1_all.deb ...
Unpacking suricata-oinkmaster (1:4.1.2-2+deb10u1) ...
Setting up libhtp2 (1:0.5.30-1) ...
Setting up libfont-afm-perl (1.20-2) ...
Setting up libyaml-0-2:amd64 (0.2.1-1) ...
Setting up libhtml-tagset-perl (3.20-3) ...
Setting up libauthen-sasl-perl (2.1600-1) ...
Setting up liblwp-mediatypes-perl (6.02-1) ...
Setting up libtry-tiny-perl (0.30-1) ...
Setting up perl-openssl-defaults:amd64 (3) ...
Setting up libencode-locale-perl (1.05-1) ...
Setting up libnet1:amd64 (1.1.6+dfsg-3.1) ...
Setting up libhyperscan5 (5.1.0-1) ...
Setting up libjansson4:amd64 (2.12-1) ...
Setting up libpython2.7-stdlib:amd64 (2.7.16-2+deb10u3) ...
Setting up libdata-dump-perl (1.23-1) ...
Setting up libnspr4:amd64 (2:4.20-1) ...
Setting up libluajit-5.1-common (2.1.0~beta3+dfsg-5.1) ...
Setting up libio-html-perl (1.001-1) ...
Setting up libltdl7:amd64 (2.4.6-9) ...
Setting up libevent-core-2.1-6:amd64 (2.1.8-stable-4) ...
Setting up libevent-2.1-6:amd64 (2.1.8-stable-4) ...
Setting up libtimedate-perl (2.3000-2+deb10u1) ...
Setting up libnfnetlink0:amd64 (1.0.1-3+b1) ...
Setting up libgeoip1:amd64 (1.6.12-1) ...
Setting up snort-rules-default (2.9.20-0+deb10u1) ...
Setting up geoip-database (20181108-1) ...
Setting up liburi-perl (1.76-1) ...
Setting up libhiredis0.14:amd64 (0.14.0-3) ...
Setting up libnet-ssleay-perl (1.85-2+deb10u1) ...
Setting up libnetfilter-log1:amd64 (1.0.1-1.1+b1) ...
Setting up libevent-pthreads-2.1-6:amd64 (2.1.8-stable-4) ...
Setting up libhttp-date-perl (6.02-1) ...
Setting up libprelude23:amd64 (4.1.0-4.2) ...
Setting up libfile-listing-perl (6.04-1) ...
Setting up python2.7 (2.7.16-2+deb10u3) ...
Setting up libpython2-stdlib:amd64 (2.7.16-1) ...
Setting up prelude-utils (4.1.0-4.2) ...
Setting up libnet-http-perl (6.18-1) ...
Setting up libnss3:amd64 (2:3.42.1-1+deb10u7) ...
Setting up python2 (2.7.16-1) ...
Setting up libluajit-5.1-2:amd64 (2.1.0~beta3+dfsg-5.1) ...
Setting up libpython-stdlib:amd64 (2.7.16-1) ...
Setting up libnetfilter-queue1 (1.0.3-1) ...
Setting up libwww-robotrules-perl (6.02-1) ...
Setting up libhtml-parser-perl (3.72-3+b3) ...
Setting up python (2.7.16-1) ...
Setting up libio-socket-ssl-perl (2.060-3) ...
Setting up libhttp-message-perl (6.18-1) ...
Setting up libhtml-form-perl (6.03-1) ...
Setting up libhttp-negotiate-perl (6.01-1) ...
Setting up libhttp-cookies-perl (6.04-1) ...
Setting up libhtml-tree-perl (5.07-2) ...
Setting up libhtml-format-perl (2.12-1) ...
Setting up python-simplejson (3.16.0-1) ...
Setting up libnet-smtp-ssl-perl (1.04-1) ...
Setting up libmailtools-perl (2.18-1) ...
Setting up suricata (1:4.1.2-2+deb10u1) ...
invoke-rc.d: could not determine current runlevel
invoke-rc.d: policy-rc.d denied execution of start.
Created symlink /etc/systemd/system/multi-user.target.wants/suricata.service → /lib/systemd/system/suricata.service.
Setting up libhttp-daemon-perl (6.01-3+deb10u1) ...
Setting up libwww-perl (6.36-2) ...
Setting up oinkmaster (2.0-4) ...
Setting up liblwp-protocol-https-perl (6.07-2) ...
Setting up suricata-oinkmaster (1:4.1.2-2+deb10u1) ...
Processing triggers for mime-support (3.62) ...
Processing triggers for libc-bin (2.28-10+deb10u2) ...
Processing triggers for systemd (241-7~deb10u8) ...
Processing triggers for man-db (2.8.5-2) ...
analyst@e980ac1fd1be:~$ apt list --installed 
Listing... Done
adduser/oldoldstable,now 3.118 all [installed,automatic]
apt/oldoldstable,oldoldstable-updates,now 1.8.2.3 amd64 [installed,automatic]
base-files/oldoldstable,now 10.3+deb10u13 amd64 [installed,automatic]
base-passwd/oldoldstable,now 3.5.46 amd64 [installed,automatic]
bash/oldoldstable,now 5.0-4 amd64 [installed,automatic]
binutils-common/oldoldstable,now 2.31.1-16 amd64 [installed,automatic]
binutils-x86-64-linux-gnu/oldoldstable,now 2.31.1-16 amd64 [installed,automatic]
binutils/oldoldstable,now 2.31.1-16 amd64 [installed,automatic]
bsdmainutils/oldoldstable,now 11.1.2+b1 amd64 [installed,automatic]
bsdutils/oldoldstable,now 1:2.33.1-0.1 amd64 [installed,automatic]
build-essential/oldoldstable,now 12.6 amd64 [installed,automatic]
bzip2/oldoldstable,now 1.0.6-9.2~deb10u2 amd64 [installed,automatic]
ca-certificates/oldoldstable,oldoldstable-updates,now 20200601~deb10u2 all [installed,automatic]
coreutils/oldoldstable,now 8.30-3 amd64 [installed,automatic]
cpp-8/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
cpp/oldoldstable,now 4:8.3.0-1 amd64 [installed,automatic]
dash/oldoldstable,now 0.5.10.2-5 amd64 [installed,automatic]
dbus/now 1.12.24-0+deb10u1 amd64 [installed,upgradable to: 1.12.28-0+deb10u1]
debconf/oldoldstable,now 1.5.71+deb10u1 all [installed,automatic]
debian-archive-keyring/oldoldstable,now 2019.1+deb10u1 all [installed,upgradable to: 2019.1+deb10u2]
debianutils/oldoldstable,now 4.8.6.1 amd64 [installed,automatic]
dh-python/oldoldstable,now 3.20190308 all [installed,automatic]
diffutils/oldoldstable,now 1:3.7-3 amd64 [installed,automatic]
dirmngr/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
dmsetup/oldoldstable,now 2:1.02.155-3 amd64 [installed,automatic]
dpkg-dev/oldoldstable,oldoldstable,now 1.19.8 all [installed,automatic]
dpkg/oldoldstable,oldoldstable,now 1.19.8 amd64 [installed,automatic]
e2fsprogs/oldoldstable,now 1.44.5-1+deb10u3 amd64 [installed,automatic]
fakeroot/oldoldstable,now 1.23-1 amd64 [installed,automatic]
fdisk/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
file/oldoldstable,now 1:5.35-4+deb10u2 amd64 [installed,automatic]
findutils/oldoldstable,now 4.6.0+git+20190209-2 amd64 [installed,automatic]
g++-8/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
g++/oldoldstable,now 4:8.3.0-1 amd64 [installed,automatic]
gcc-8-base/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
gcc-8/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
gcc/oldoldstable,now 4:8.3.0-1 amd64 [installed,automatic]
geoip-database/oldoldstable,now 20181108-1 all [installed,automatic]
gir1.2-glib-2.0/oldoldstable,now 1.58.3-2 amd64 [installed,automatic]
gnupg-l10n/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 all [installed,automatic]
gnupg-utils/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gnupg/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 all [installed,automatic]
gpg-agent/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gpg-wks-client/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gpg-wks-server/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gpg/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gpgconf/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gpgsm/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
gpgv/oldoldstable,oldoldstable,now 2.2.12-1+deb10u2 amd64 [installed,automatic]
grep/oldoldstable,now 3.3-1 amd64 [installed,automatic]
groff-base/oldoldstable,now 1.22.4-3+deb10u1 amd64 [installed,automatic]
gzip/oldoldstable,oldoldstable,now 1.9-3+deb10u1 amd64 [installed,automatic]
hostname/oldoldstable,now 3.21 amd64 [installed,automatic]
info/oldoldstable,now 6.5.0.dfsg.1-4+b1 amd64 [installed]
init-system-helpers/oldoldstable,now 1.56+nmu1 all [installed,automatic]
install-info/oldoldstable,now 6.5.0.dfsg.1-4+b1 amd64 [installed,automatic]
iproute2/oldoldstable,now 4.20.0-2+deb10u1 amd64 [installed]
iputils-ping/oldoldstable,now 3:20180629-2+deb10u2 amd64 [installed]
krb5-locales/now 1.17-3+deb10u5 all [installed,upgradable to: 1.17-3+deb10u6]
libacl1/oldoldstable,now 2.2.53-4 amd64 [installed,automatic]
libalgorithm-diff-perl/oldoldstable,now 1.19.03-2 all [installed,automatic]
libalgorithm-diff-xs-perl/oldoldstable,now 0.04-5+b1 amd64 [installed,automatic]
libalgorithm-merge-perl/oldoldstable,now 0.08-3 all [installed,automatic]
libapparmor1/oldoldstable,now 2.13.2-10 amd64 [installed,automatic]
libapt-pkg5.0/oldoldstable,oldoldstable-updates,now 1.8.2.3 amd64 [installed,automatic]
libargon2-1/oldoldstable,now 0~20171227-0.2 amd64 [installed,automatic]
libasan5/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libassuan0/oldoldstable,now 2.5.2-1 amd64 [installed,automatic]
libatomic1/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libattr1/oldoldstable,now 1:2.4.48-4 amd64 [installed,automatic]
libaudit-common/oldoldstable,now 1:2.8.4-3 all [installed,automatic]
libaudit1/oldoldstable,now 1:2.8.4-3 amd64 [installed,automatic]
libauthen-sasl-perl/oldoldstable,now 2.1600-1 all [installed,automatic]
libbinutils/oldoldstable,now 2.31.1-16 amd64 [installed,automatic]
libblkid1/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
libbsd0/oldoldstable,now 0.9.1-2+deb10u1 amd64 [installed,automatic]
libbz2-1.0/oldoldstable,now 1.0.6-9.2~deb10u2 amd64 [installed,automatic]
libc-bin/oldoldstable,now 2.28-10+deb10u2 amd64 [installed,automatic]
libc-dev-bin/oldoldstable,now 2.28-10+deb10u2 amd64 [installed,automatic]
libc6-dev/oldoldstable,now 2.28-10+deb10u2 amd64 [installed,automatic]
libc6/oldoldstable,now 2.28-10+deb10u2 amd64 [installed,automatic]
libcap-ng0/oldoldstable,now 0.7.9-2 amd64 [installed,automatic]
libcap2-bin/oldoldstable,now 1:2.25-2 amd64 [installed,automatic]
libcap2/oldoldstable,now 1:2.25-2 amd64 [installed,automatic]
libcc1-0/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libcom-err2/oldoldstable,now 1.44.5-1+deb10u3 amd64 [installed,automatic]
libcryptsetup12/oldoldstable,now 2:2.1.0-5+deb10u2 amd64 [installed,automatic]
libdata-dump-perl/oldoldstable,now 1.23-1 all [installed,automatic]
libdb5.3/oldoldstable,now 5.3.28+dfsg1-0.5 amd64 [installed,automatic]
libdbus-1-3/now 1.12.24-0+deb10u1 amd64 [installed,upgradable to: 1.12.28-0+deb10u1]
libdebconfclient0/oldoldstable,now 0.249 amd64 [installed,automatic]
libdevmapper1.02.1/oldoldstable,now 2:1.02.155-3 amd64 [installed,automatic]
libdpkg-perl/oldoldstable,oldoldstable,now 1.19.8 all [installed,automatic]
libedit2/oldoldstable,now 3.1-20181209-1 amd64 [installed,automatic]
libelf1/oldoldstable,now 0.176-1.1 amd64 [installed,upgradable to: 0.176-1.1+deb10u1]
libencode-locale-perl/oldoldstable,now 1.05-1 all [installed,automatic]
libevent-2.1-6/oldoldstable,now 2.1.8-stable-4 amd64 [installed,automatic]
libevent-core-2.1-6/oldoldstable,now 2.1.8-stable-4 amd64 [installed,automatic]
libevent-pthreads-2.1-6/oldoldstable,now 2.1.8-stable-4 amd64 [installed,automatic]
libexpat1-dev/oldoldstable,now 2.2.6-2+deb10u6 amd64 [installed,automatic]
libexpat1/oldoldstable,now 2.2.6-2+deb10u6 amd64 [installed,automatic]
libext2fs2/oldoldstable,now 1.44.5-1+deb10u3 amd64 [installed,automatic]
libfakeroot/oldoldstable,now 1.23-1 amd64 [installed,automatic]
libfdisk1/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
libffi6/oldoldstable,now 3.2.1-9 amd64 [installed,automatic]
libfile-fcntllock-perl/oldoldstable,now 0.22-3+b5 amd64 [installed,automatic]
libfile-listing-perl/oldoldstable,now 6.04-1 all [installed,automatic]
libfont-afm-perl/oldoldstable,now 1.20-2 all [installed,automatic]
libgcc-8-dev/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libgcc1/oldoldstable,now 1:8.3.0-6 amd64 [installed,automatic]
libgcrypt20/oldoldstable,now 1.8.4-5+deb10u1 amd64 [installed,automatic]
libgdbm-compat4/oldoldstable,now 1.18.1-4 amd64 [installed,automatic]
libgdbm6/oldoldstable,now 1.18.1-4 amd64 [installed,automatic]
libgeoip1/oldoldstable,now 1.6.12-1 amd64 [installed,automatic]
libgirepository-1.0-1/oldoldstable,now 1.58.3-2 amd64 [installed,automatic]
libglib2.0-0/now 2.58.3-2+deb10u4 amd64 [installed,upgradable to: 2.58.3-2+deb10u5]
libglib2.0-data/now 2.58.3-2+deb10u4 all [installed,upgradable to: 2.58.3-2+deb10u5]
libgmp10/oldoldstable,now 2:6.1.2+dfsg-4+deb10u1 amd64 [installed,automatic]
libgnutls30/now 3.6.7-4+deb10u10 amd64 [installed,upgradable to: 3.6.7-4+deb10u11]
libgomp1/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libgpg-error0/oldoldstable,now 1.35-1 amd64 [installed,automatic]
libgpm2/oldoldstable,now 1.20.7-5 amd64 [installed,automatic]
libgssapi-krb5-2/now 1.17-3+deb10u5 amd64 [installed,upgradable to: 1.17-3+deb10u6]
libhiredis0.14/oldoldstable,now 0.14.0-3 amd64 [installed,automatic]
libhogweed4/oldoldstable,oldoldstable,now 3.4.1-1+deb10u1 amd64 [installed,automatic]
libhtml-form-perl/oldoldstable,now 6.03-1 all [installed,automatic]
libhtml-format-perl/oldoldstable,now 2.12-1 all [installed,automatic]
libhtml-parser-perl/oldoldstable,now 3.72-3+b3 amd64 [installed,automatic]
libhtml-tagset-perl/oldoldstable,now 3.20-3 all [installed,automatic]
libhtml-tree-perl/oldoldstable,now 5.07-2 all [installed,automatic]
libhtp2/oldoldstable,now 1:0.5.30-1 amd64 [installed,automatic]
libhttp-cookies-perl/oldoldstable,now 6.04-1 all [installed,automatic]
libhttp-daemon-perl/oldoldstable,now 6.01-3+deb10u1 all [installed,automatic]
libhttp-date-perl/oldoldstable,now 6.02-1 all [installed,automatic]
libhttp-message-perl/oldoldstable,now 6.18-1 all [installed,automatic]
libhttp-negotiate-perl/oldoldstable,now 6.01-1 all [installed,automatic]
libhyperscan5/oldoldstable,now 5.1.0-1 amd64 [installed,automatic]
libicu63/oldoldstable,now 63.1-6+deb10u3 amd64 [installed,automatic]
libidn11/oldoldstable,now 1.33-2.2 amd64 [installed,automatic]
libidn2-0/oldoldstable,oldoldstable,now 2.0.5-1+deb10u1 amd64 [installed,automatic]
libio-html-perl/oldoldstable,now 1.001-1 all [installed,automatic]
libio-socket-ssl-perl/oldoldstable,now 2.060-3 all [installed,automatic]
libip4tc0/oldoldstable,now 1.8.2-4 amd64 [installed,automatic]
libisl19/oldoldstable,now 0.20-2 amd64 [installed,automatic]
libitm1/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libjansson4/oldoldstable,now 2.12-1 amd64 [installed,automatic]
libjson-c3/oldoldstable,oldoldstable,now 0.12.1+ds-2+deb10u1 amd64 [installed,automatic]
libk5crypto3/now 1.17-3+deb10u5 amd64 [installed,upgradable to: 1.17-3+deb10u6]
libkeyutils1/oldoldstable,now 1.6-6 amd64 [installed,automatic]
libkmod2/oldoldstable,now 26-1 amd64 [installed,automatic]
libkrb5-3/now 1.17-3+deb10u5 amd64 [installed,upgradable to: 1.17-3+deb10u6]
libkrb5support0/now 1.17-3+deb10u5 amd64 [installed,upgradable to: 1.17-3+deb10u6]
libksba8/oldoldstable,now 1.3.5-2+deb10u2 amd64 [installed,automatic]
libldap-2.4-2/oldoldstable,oldoldstable,now 2.4.47+dfsg-3+deb10u7 amd64 [installed,automatic]
libldap-common/oldoldstable,oldoldstable,now 2.4.47+dfsg-3+deb10u7 all [installed,automatic]
liblocale-gettext-perl/oldoldstable,now 1.07-3+b4 amd64 [installed,automatic]
liblsan0/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libltdl7/oldoldstable,now 2.4.6-9 amd64 [installed,automatic]
libluajit-5.1-2/oldoldstable,now 2.1.0~beta3+dfsg-5.1 amd64 [installed,automatic]
libluajit-5.1-common/oldoldstable,now 2.1.0~beta3+dfsg-5.1 all [installed,automatic]
liblwp-mediatypes-perl/oldoldstable,now 6.02-1 all [installed,automatic]
liblwp-protocol-https-perl/oldoldstable,now 6.07-2 all [installed,automatic]
liblz4-1/oldoldstable,oldoldstable,now 1.8.3-1+deb10u1 amd64 [installed,automatic]
liblzma5/oldoldstable,oldoldstable,now 5.2.4-1+deb10u1 amd64 [installed,automatic]
libmagic-mgc/oldoldstable,now 1:5.35-4+deb10u2 amd64 [installed,automatic]
libmagic1/oldoldstable,now 1:5.35-4+deb10u2 amd64 [installed,automatic]
libmailtools-perl/oldoldstable,now 2.18-1 all [installed,automatic]
libmnl0/oldoldstable,now 1.0.4-2 amd64 [installed,automatic]
libmount1/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
libmpc3/oldoldstable,now 1.1.0-1 amd64 [installed,automatic]
libmpdec2/oldoldstable,now 2.4.2-2 amd64 [installed,automatic]
libmpfr6/oldoldstable,now 4.0.2-1 amd64 [installed,automatic]
libmpx2/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libncurses6/now 6.1+20181013-2+deb10u3 amd64 [installed,upgradable to: 6.1+20181013-2+deb10u5]
libncursesw6/now 6.1+20181013-2+deb10u3 amd64 [installed,upgradable to: 6.1+20181013-2+deb10u5]
libnet-http-perl/oldoldstable,now 6.18-1 all [installed,automatic]
libnet-smtp-ssl-perl/oldoldstable,now 1.04-1 all [installed,automatic]
libnet-ssleay-perl/oldoldstable,now 1.85-2+deb10u1 amd64 [installed,automatic]
libnet1/oldoldstable,now 1.1.6+dfsg-3.1 amd64 [installed,automatic]
libnetfilter-log1/oldoldstable,now 1.0.1-1.1+b1 amd64 [installed,automatic]
libnetfilter-queue1/oldoldstable,now 1.0.3-1 amd64 [installed,automatic]
libnettle6/oldoldstable,oldoldstable,now 3.4.1-1+deb10u1 amd64 [installed,automatic]
libnfnetlink0/oldoldstable,now 1.0.1-3+b1 amd64 [installed,automatic]
libnpth0/oldoldstable,now 1.6-1 amd64 [installed,automatic]
libnspr4/oldoldstable,now 2:4.20-1 amd64 [installed,automatic]
libnss-systemd/oldoldstable,now 241-7~deb10u8 amd64 [installed,upgradable to: 241-7~deb10u10]
libnss3/oldoldstable,now 2:3.42.1-1+deb10u7 amd64 [installed,automatic]
libp11-kit0/oldoldstable,oldoldstable,now 0.23.15-2+deb10u1 amd64 [installed,automatic]
libpam-modules-bin/oldoldstable,now 1.3.1-5 amd64 [installed,automatic]
libpam-modules/oldoldstable,now 1.3.1-5 amd64 [installed,automatic]
libpam-runtime/oldoldstable,now 1.3.1-5 all [installed,automatic]
libpam-systemd/oldoldstable,now 241-7~deb10u8 amd64 [installed,upgradable to: 241-7~deb10u10]
libpam0g/oldoldstable,now 1.3.1-5 amd64 [installed,automatic]
libpcap0.8/oldoldstable,now 1.8.1-6+deb10u1 amd64 [installed,automatic]
libpcre2-8-0/oldoldstable,now 10.32-5 amd64 [installed,upgradable to: 10.32-5+deb10u1]
libpcre3/oldoldstable,now 2:8.39-12 amd64 [installed,automatic]
libperl5.28/oldoldstable,now 5.28.1-6+deb10u1 amd64 [installed,automatic]
libpipeline1/oldoldstable,now 1.5.1-2 amd64 [installed,automatic]
libprelude23/oldoldstable,now 4.1.0-4.2 amd64 [installed,automatic]
libprocps7/oldoldstable,now 2:3.3.15-2 amd64 [installed,automatic]
libpsl5/oldoldstable,now 0.20.2-2 amd64 [installed,automatic]
libpython-stdlib/oldoldstable,now 2.7.16-1 amd64 [installed,automatic]
libpython2-stdlib/oldoldstable,now 2.7.16-1 amd64 [installed,automatic]
libpython2.7-minimal/oldoldstable,now 2.7.16-2+deb10u3 amd64 [installed,automatic]
libpython2.7-stdlib/oldoldstable,now 2.7.16-2+deb10u3 amd64 [installed,automatic]
libpython3-dev/oldoldstable,now 3.7.3-1 amd64 [installed,automatic]
libpython3-stdlib/oldoldstable,now 3.7.3-1 amd64 [installed,automatic]
libpython3.7-dev/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
libpython3.7-minimal/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
libpython3.7-stdlib/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
libpython3.7/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
libquadmath0/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libreadline7/oldoldstable,now 7.0-5 amd64 [installed,automatic]
libsasl2-2/oldoldstable,oldoldstable,now 2.1.27+dfsg-1+deb10u2 amd64 [installed,automatic]
libsasl2-modules-db/oldoldstable,oldoldstable,now 2.1.27+dfsg-1+deb10u2 amd64 [installed,automatic]
libsasl2-modules/oldoldstable,oldoldstable,now 2.1.27+dfsg-1+deb10u2 amd64 [installed,automatic]
libseccomp2/oldoldstable,now 2.3.3-4 amd64 [installed,automatic]
libselinux1/oldoldstable,now 2.8-1+b1 amd64 [installed,automatic]
libsemanage-common/oldoldstable,now 2.8-2 all [installed,automatic]
libsemanage1/oldoldstable,now 2.8-2 amd64 [installed,automatic]
libsepol1/oldoldstable,now 2.8-1 amd64 [installed,automatic]
libsmartcols1/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
libsqlite3-0/oldoldstable,now 3.27.2-3+deb10u2 amd64 [installed,automatic]
libss2/oldoldstable,now 1.44.5-1+deb10u3 amd64 [installed,automatic]
libssl1.1/now 1.1.1n-0+deb10u4 amd64 [installed,upgradable to: 1.1.1n-0+deb10u6]
libstdc++-8-dev/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libstdc++6/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libsystemd0/oldoldstable,now 241-7~deb10u8 amd64 [installed,upgradable to: 241-7~deb10u10]
libtasn1-6/oldoldstable,now 4.13-3+deb10u1 amd64 [installed,automatic]
libtimedate-perl/oldoldstable,now 2.3000-2+deb10u1 all [installed,automatic]
libtinfo6/now 6.1+20181013-2+deb10u3 amd64 [installed,upgradable to: 6.1+20181013-2+deb10u5]
libtry-tiny-perl/oldoldstable,now 0.30-1 all [installed,automatic]
libtsan0/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libubsan1/oldoldstable,now 8.3.0-6 amd64 [installed,automatic]
libuchardet0/oldoldstable,now 0.0.6-3 amd64 [installed,automatic]
libudev1/oldoldstable,now 241-7~deb10u8 amd64 [installed,upgradable to: 241-7~deb10u10]
libunistring2/oldoldstable,now 0.9.10-1 amd64 [installed,automatic]
liburi-perl/oldoldstable,now 1.76-1 all [installed,automatic]
libuuid1/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
libwrap0/oldoldstable,now 7.6.q-28 amd64 [installed,automatic]
libwww-perl/oldoldstable,now 6.36-2 all [installed,automatic]
libwww-robotrules-perl/oldoldstable,now 6.02-1 all [installed,automatic]
libx11-6/oldoldstable,now 2:1.6.7-1+deb10u2 amd64 [installed,upgradable to: 2:1.6.7-1+deb10u4]
libx11-data/oldoldstable,now 2:1.6.7-1+deb10u2 all [installed,upgradable to: 2:1.6.7-1+deb10u4]
libxau6/oldoldstable,now 1:1.0.8-1+b2 amd64 [installed,automatic]
libxcb1/oldoldstable,now 1.13.1-2 amd64 [installed,automatic]
libxdmcp6/oldoldstable,now 1:1.1.2-3 amd64 [installed,automatic]
libxext6/oldoldstable,now 2:1.3.3-1+b2 amd64 [installed,automatic]
libxml2/now 2.9.4+dfsg1-7+deb10u5 amd64 [installed,upgradable to: 2.9.4+dfsg1-7+deb10u6]
libxmuu1/oldoldstable,now 2:1.1.2-2+b3 amd64 [installed,automatic]
libxtables12/oldoldstable,now 1.8.2-4 amd64 [installed,automatic]
libyaml-0-2/oldoldstable,now 0.2.1-1 amd64 [installed,automatic]
libzstd1/oldoldstable,oldoldstable,now 1.3.8+dfsg-3+deb10u2 amd64 [installed,automatic]
linux-libc-dev/now 4.19.269-1 amd64 [installed,upgradable to: 4.19.289-2]
login/oldoldstable,now 1:4.5-1.1 amd64 [installed,automatic]
lsb-base/oldoldstable,now 10.2019051400 all [installed,automatic]
make/oldoldstable,now 4.2.1-1.2 amd64 [installed,automatic]
man-db/oldoldstable,now 2.8.5-2 amd64 [installed]
manpages-dev/oldoldstable,now 4.16-2 all [installed,automatic]
manpages/oldoldstable,now 4.16-2 all [installed,automatic]
mawk/oldoldstable,now 1.3.3-17+b3 amd64 [installed,automatic]
mime-support/oldoldstable,now 3.62 all [installed,automatic]
mount/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
nano/oldoldstable,now 3.2-3 amd64 [installed]
ncurses-base/now 6.1+20181013-2+deb10u3 all [installed,upgradable to: 6.1+20181013-2+deb10u5]
ncurses-bin/now 6.1+20181013-2+deb10u3 amd64 [installed,upgradable to: 6.1+20181013-2+deb10u5]
ncurses-term/now 6.1+20181013-2+deb10u3 all [installed,upgradable to: 6.1+20181013-2+deb10u5]
netbase/oldoldstable,now 5.6 all [installed,automatic]
oinkmaster/oldoldstable,now 2.0-4 all [installed,automatic]
openssh-client/oldoldstable,now 1:7.9p1-10+deb10u2 amd64 [installed,upgradable to: 1:7.9p1-10+deb10u3]
openssh-server/oldoldstable,now 1:7.9p1-10+deb10u2 amd64 [installed,upgradable to: 1:7.9p1-10+deb10u3]
openssh-sftp-server/oldoldstable,now 1:7.9p1-10+deb10u2 amd64 [installed,upgradable to: 1:7.9p1-10+deb10u3]
openssl/now 1.1.1n-0+deb10u4 amd64 [installed,upgradable to: 1.1.1n-0+deb10u6]
passwd/oldoldstable,now 1:4.5-1.1 amd64 [installed,automatic]
patch/oldoldstable,oldoldstable,now 2.7.6-3+deb10u1 amd64 [installed,automatic]
perl-base/oldoldstable,now 5.28.1-6+deb10u1 amd64 [installed,automatic]
perl-modules-5.28/oldoldstable,now 5.28.1-6+deb10u1 all [installed,automatic]
perl-openssl-defaults/oldoldstable,now 3 amd64 [installed,automatic]
perl/oldoldstable,now 5.28.1-6+deb10u1 amd64 [installed,automatic]
pinentry-curses/oldoldstable,now 1.1.0-2 amd64 [installed,automatic]
prelude-utils/oldoldstable,now 4.1.0-4.2 amd64 [installed,automatic]
procps/oldoldstable,now 2:3.3.15-2 amd64 [installed,automatic]
psmisc/oldoldstable,now 23.2-1+deb10u1 amd64 [installed,automatic]
publicsuffix/oldoldstable,now 20220811.1734-0+deb10u1 all [installed,automatic]
python-minimal/oldoldstable,now 2.7.16-1 amd64 [installed,automatic]
python-pip-whl/oldoldstable,now 18.1-5 all [installed,automatic]
python-simplejson/oldoldstable,now 3.16.0-1 amd64 [installed,automatic]
python2-minimal/oldoldstable,now 2.7.16-1 amd64 [installed,automatic]
python2.7-minimal/oldoldstable,now 2.7.16-2+deb10u3 amd64 [installed,automatic]
python2.7/oldoldstable,now 2.7.16-2+deb10u3 amd64 [installed,automatic]
python2/oldoldstable,now 2.7.16-1 amd64 [installed,automatic]
python3-asn1crypto/oldoldstable,now 0.24.0-1 all [installed,automatic]
python3-cffi-backend/oldoldstable,now 1.12.2-1 amd64 [installed,automatic]
python3-crypto/oldoldstable,now 2.6.1-9+b1 amd64 [installed,automatic]
python3-cryptography/oldoldstable,now 2.6.1-3+deb10u4 amd64 [installed,automatic]
python3-dbus/oldoldstable,now 1.2.8-3 amd64 [installed,automatic]
python3-dev/oldoldstable,now 3.7.3-1 amd64 [installed,automatic]
python3-distutils/oldoldstable,now 3.7.3-1 all [installed,automatic]
python3-entrypoints/oldoldstable,now 0.3-1 all [installed,automatic]
python3-gi/oldoldstable,now 3.30.4-1 amd64 [installed,automatic]
python3-keyring/oldoldstable,now 17.1.1-1 all [installed,automatic]
python3-keyrings.alt/oldoldstable,now 3.1.1-1 all [installed,automatic]
python3-lib2to3/oldoldstable,now 3.7.3-1 all [installed,automatic]
python3-minimal/oldoldstable,now 3.7.3-1 amd64 [installed,automatic]
python3-pip/oldoldstable,now 18.1-5 all [installed]
python3-pkg-resources/oldoldstable,now 40.8.0-1 all [installed,automatic]
python3-secretstorage/oldoldstable,now 2.3.1-2 all [installed,automatic]
python3-setuptools/oldoldstable,now 40.8.0-1 all [installed,automatic]
python3-six/oldoldstable,now 1.12.0-1 all [installed,automatic]
python3-wheel/oldoldstable,now 0.32.3-2 all [installed,automatic]
python3-xdg/oldoldstable,now 0.25-5 all [installed,automatic]
python3.7-dev/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
python3.7-minimal/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
python3.7/now 3.7.3-2+deb10u4 amd64 [installed,upgradable to: 3.7.3-2+deb10u6]
python3/oldoldstable,now 3.7.3-1 amd64 [installed]
python/oldoldstable,now 2.7.16-1 amd64 [installed,automatic]
readline-common/oldoldstable,now 7.0-5 all [installed,automatic]
sed/oldoldstable,now 4.7-1 amd64 [installed,automatic]
sensible-utils/oldoldstable,now 0.0.12 all [installed,automatic]
shared-mime-info/oldoldstable,now 1.10-1 amd64 [installed,automatic]
snort-rules-default/oldoldstable,now 2.9.20-0+deb10u1 all [installed,automatic]
sudo/oldoldstable,now 1.8.27-1+deb10u5 amd64 [installed]
suricata-oinkmaster/oldoldstable,now 1:4.1.2-2+deb10u1 all [installed,automatic]
suricata/oldoldstable,now 1:4.1.2-2+deb10u1 amd64 [installed]
systemd-sysv/oldoldstable,now 241-7~deb10u8 amd64 [installed,upgradable to: 241-7~deb10u10]
systemd/oldoldstable,now 241-7~deb10u8 amd64 [installed,upgradable to: 241-7~deb10u10]
sysvinit-utils/oldoldstable,now 2.93-8 amd64 [installed,automatic]
tar/oldoldstable,now 1.30+dfsg-6 amd64 [installed,automatic]
tcpdump/oldoldstable,now 4.9.3-1~deb10u2 amd64 [installed]
tree/oldoldstable,now 1.8.0-1 amd64 [installed]
tzdata/now 2021a-0+deb10u8 all [installed,upgradable to: 2021a-0+deb10u12]
ucf/oldoldstable,now 3.0038+nmu1 all [installed,automatic]
util-linux/oldoldstable,now 2.33.1-0.1 amd64 [installed,automatic]
wget/oldoldstable,now 1.20.1-1.1 amd64 [installed]
xauth/oldoldstable,now 1:1.0.10-1 amd64 [installed,automatic]
xdg-user-dirs/oldoldstable,now 0.17-2 amd64 [installed,automatic]
xz-utils/oldoldstable,oldoldstable,now 5.2.4-1+deb10u1 amd64 [installed,automatic]
zlib1g/oldoldstable,now 1:1.2.11.dfsg-1+deb10u2 amd64 [installed,automatic]
