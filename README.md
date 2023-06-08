# raspi_wap
Raspberry Pi OS WAP setup


## Genral Setup

`sudo raspi-config`
- Select __Advanced Options__
- Select __Network Manager__

Plug in ethernet and establish connection

Via Netowrk Manager activate WiFi hotspot and set it connect on boot


## Options

- Setup MQTT broker
  - `sudo nano /etc/mosquitto/mosquitto.conf`

- Setup nodejs express web-server
  - [https://nvm.sh](https://nvm.sh)
  - 
