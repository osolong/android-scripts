#cfgandroid
Ubuntu Configuration Script to setup Android Development Environment

##Version
0.2

##Description
Make sure and repo links are up to date before running this script

Configures an ubuntu host PC. Will perform the following actions:
  - Setup Git
  - Create ssh RSA key
  - Create udev rules to conenct an android device.
  - Download the latest repo tool
  - Install a TFTP server
  - Install the requirements for building android.

##Instructions
On a brand new Ubuntu 14.04 installation run the following commands
```
sudo apt-get install git-core
cd; mkdir -p bin; cd bin
wget https://raw.githubusercontent.com/osolong/android-scripts/master/cfgandroid
chmod +x cfgandroid
sudo ./cfgandroid
```

##Packages to be installed:
```
	pkgs="
		git-core \
		gnupg 	\
		flex 	\
		bison 	\
		gperf 	\
		build-essential \
		zip 	\
		curl 	\
		libc6-dev \
		libncurses5-dev:i386 \
		x11proto-core-dev \
		libx11-dev:i386 \
		libreadline6-dev:i386 \
		libgl1-mesa-dev \
		g++-multilib \
		mingw32 \
		tofrodos \
		python-markdown \
		libxml2-utils \
		xsltproc \
		zlib1g-dev:i386 \
		cramfsprogs \
		squashfs-tools \
		eclipse \
		u-boot-tools \
		gitk \
		tftp-hpa \
		indent \
		multistrap \
		netpbm \
		tofrodos \
		gawk \
		chrpath \
		quilt \
		dpkg-dev \
		debhelper \
		autoconf \
		libtool \
		mercurial \
		intltool \
		vim \
		vim-common \
		vim-gnome \
		vim-gui-common \
		vim-runtime \
		exuberant-ctags \
		cscope \
		android-tools-adb \
		android-tools-fastboot \
		android-tools-fsutils \
		oracle-java6-installer \
		openjdk-7-jdk \
		"
```
