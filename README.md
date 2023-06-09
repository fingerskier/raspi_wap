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
