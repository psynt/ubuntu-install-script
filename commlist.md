
wget -nv http://download.opensuse.org/repositories/isv:ownCloud:desktop/Ubuntu_17.04/Release.key -O Release.key
wget https://raw.githubusercontent.com/quidsup/flashless-extras/master/flashless.sh
curl -s https://packagecloud.io/install/repositories/github/git-lfs/script.deb.sh | sudo bash
sudo apt-key add - < Release.key
rm Release.key
sudo add-apt-repository ppa:maarten-baert/simplescreenrecorder
sudo add-apt-repository ppa:webupd8team/java
wget https://launchpad.net/~kxstudio-debian/+archive/kxstudio/+files/kxstudio-repos_9.4.6~kxstudio1_all.deb
sudo dpkg -i kxstudio-repos_9.4.6~kxstudio1_all.deb
rm kxstudio-repos_9.4.6~kxstudio1_all.deb
sudo add-apt-repository ppa:kubuntu-ppa/ppa
sudo add-apt-repository ppa:kubuntu-ppa/backports


sudo apt update
sudo apt upgrade

sudo apt install g++ --install-suggests
sudo apt install curl
sudo apt install libdvd-pkg
sudo apt install --install-suggests git-all
sudo apt install git-lfs
sudo apt install --install-suggests ibus anthy kasumi ibus-anthy ibus-gtk* ibus-qt4
sudo apt install --install-suggests anki
sudo apt install steam slack texmaker
sudo apt install owncloud-client
sudo apt install ssh samba
sudo apt install --install-suggests aptitude virtualbox virtualbox-ext-pack
sudo apt install mtpfs mtp-tools
sudo apt install gufw
sudo apt install htop redshift-gtk shutter

##sudo apt install nvidia-common nvidia-375 bumblebee-nvidia

sudo apt install evince clementine
sudo apt install simplescreenrecorder
# if you want to record 32-bit OpenGL applications on a 64-bit system:
sudo apt install simplescreenrecorder-lib:i386
sudo apt install --install-suggests audacity
sudo apt install --install-suggests jack pulseaudio-module-jack
sudo apt install libglibmm-2.4-1v5
wget https://launchpad.net/~kxstudio-debian/+archive/kxstudio/+files/kxstudio-repos-gcc5_9.4.6~kxstudio1_all.deb
sudo dpkg -i kxstudio-repos-gcc5_9.4.6~kxstudio1_all.deb
sudo apt update
sudo apt install guitarix xjadeo libsox-fmt-all mjpegtools xvid4conf ardour
sudo apt install kxstudio-default-settings kxstudio-welcome kxstudio-meta-all
sudo apt install konqueror konq-plugins
sudo apt install kxstudio-meta-audio-plugins-ladspa ubuntustudio-audio-plugins terminatorx
sudo apt install haskell-stack
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.2/install.sh | bash


##SDKMAN

curl -s "https://get.sdkman.io" | bash
source "/home/junko/.sdkman/bin/sdkman-init.sh"
sdk i java
sdk i groovy
sdk i gradle
sdk i scala
sdk i griffon
sdk i grails
sdk i lazybones
sdk i groovyserv




