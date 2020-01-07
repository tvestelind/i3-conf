# Install #

## Debian ##
```bas
apt install i3-blocks rofi xautolock keepassxc
```

## From source
```bash
git clone https://github.com/haikarainen/light.git &&  make && sudo make install
```

### i3blocks ###
#### monitor manager ####
```bash
apt install python3 python3-tk arandr fonts-font-awesome
```

#### temp ####
```bash
apt install lm-sensors
```

#### ssid ####
```bash
sudo ln -s $(sudo which iw) /usr/bin/iw && sudo chmod +x /usr/bin/iw
```

#### mediaplayer ####
```bash
wget https://github.com/acrisci/playerctl/releases/download/v0.5.0/playerctl-0.5.0_amd64.deb
sudo dpkg -i playerctl-0.5.0_amd64.deb
rm playerctl-0.5.0_amd64.deb
```

#### contrib repo ####
```bash
git submodule init && git submodule update --recursive
```

## Fonts ##
```bash
pushd fonts && mkdir --parent ~/.local/share/fonts && cp *.ttf ~/.local/share/fonts && fc-cache -fv && popd
```

# Troubleshooting
## Components aren't working in i3blocks
* Look at `i3blocks.conf` and see what's configured to show
* Go to `i3blocks-contrib` and install dependencies for components that aren't working
