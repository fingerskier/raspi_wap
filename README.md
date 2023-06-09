# raspi_wap
Raspberry Pi OS WAP setup


## General Setup

`sudo raspi-config`
- Select __Advanced Options__
- Select __Network Manager__
- ...if it's not there you probably need to update/upgrade the system

Plug in ethernet and establish connection

Via Network Manager activate WiFi hotspot and set it connect on startup


## Options

- Setup MQTT broker
  - `sudo nano /etc/mosquitto/mosquitto.conf`

- Setup nodejs express web-server
  - [https://nvm.sh](https://nvm.sh)
  - 

- webmin

- zerotier
```
sudo apt update
sudo apt upgrade
curl https://raw.githubusercontent.com/zerotier/ZeroTierOne/master/doc/contact%40zerotier.com.gpg | gpg --dearmor | sudo tee /usr/share/keyrings/zerotierone-archive-keyring.gpg >/dev/null
RELEASE=$(lsb_release -cs)
echo "deb [signed-by=/usr/share/keyrings/zerotierone-archive-keyring.gpg] http://download.zerotier.com/debian/$RELEASE $RELEASE main" | sudo tee /etc/apt/sources.list.d/zerotier.list
sudo apt update
sudo apt install -y zerotier-one
sudo zerotier-cli join [NETWORKID]
https://my.zerotier.com/network/[NETWORKID]
sudo zerotier-cli listnetworks
```

ORIG: [https://pimylifeup.com/raspberry-pi-zerotier/](https://pimylifeup.com/raspberry-pi-zerotier/)
