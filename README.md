# Install #
## Debian ##
apt-get install i3-blocks
### i3blocks ###
#### monitor manager ####
apt-get install python3-tk arandr
#### temp ####
apt-get install lm-sensors
#### ssid ####
sudo ln -s /usr/sbin/iw /usr/bin/iw && sudo chmod +x /usr/bin/iw
#### mediaplayer ####
wget https://github.com/acrisci/playerctl/releases/download/v0.5.0/playerctl-0.5.0_amd64.deb
dpkg -i playerctl-0.5.0_amd64.deb
rm playerctl-0.5.0_amd64.deb
#### contrib repo ####
git submodule init && git submodule update --recursive
## fonts ##
pushd fonts && mkdir --parent ~/.local/share/fonts && cp *.ttf ~/.local/share/fonts && fc-cache -fv && popd
