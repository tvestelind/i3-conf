# Install #
## Debian ##
apt-get install i3-blocks curl lm-sensors python3-tk arandr
### i3blocks ###
#### monitor_manager ####
apt-get install python3-tk arandr
#### temp ####
apt-get install lm-sensors
#### ssid ####
sudo ln -s /usr/sbin/iw /usr/bin/iw && sudo chmod +x /usr/bin/iw
## fonts ##
pushd fonts && mkdir --parent ~/.local/share/fonts && cp *.ttf ~/.local/share/fonts && fc-cache -fv && popd
