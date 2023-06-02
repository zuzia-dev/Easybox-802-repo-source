# Gargoyle:1.13.X (Built 20210517-1931 git@) for Arcadyan/Astoria ARV752DPW (EasyBox 802)
[![Gargoyle](https://img.shields.io/badge/os-Gargoyle-<COLOR>.svg)](https://github.com/ericpaulbishop/gargoyle/) [![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://github.com/zuzia-dev/Easybox-904xDSL-repo-source#license) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/zuzia-dev/Easybox-802-repo-source?color=orange)](https://github.com/zuzia-dev/Easybox-802-repo-source/releases/latest) [![GitHub Downloads](https://img.shields.io/github/downloads/zuzia-dev/Easybox-802-repo-source/latest/total)](https://github.com/zuzia-dev/Easybox-802-repo-source/releases/latest)

#### Default configuration of LAN4/TV port as WAN for cable Internet connection (not included DSL software)
- Kernel version: 4.14.232
- The router address: 192.168.1.1
- Login page: http://192.168.1.1
- SSH - Username: root 
- Password (Web & SSH): password
- WiFi is active, ssid: Gargoyle
- Password: WiFipassword
- WPS button turns Wi-Fi on or off

#### GUI with internationalization and localization PL & EN
Includes:
- plugin-gargoyle-3ginfo 
- plugin-gargoyle-cron 
- plugin-gargoyle-management
- plugin-gargoyle-msg 
- plugin-gargoyle-logread
- plugin-gargoyle-initd
- plugin-gargoyle-management
- plugin-gargoyle-msg 
- plugin-gargoyle-qos
- plugin-gargoyle-ping-watchdog
- plugin-gargoyle-stamgr
- plugin-gargoyle-spectrum-analyser-minimal
- plugin-gargoyle-webshell
- plugin-gargoyle-wifi-scheduler
- plugin-gargoyle-usb-storage-noshare 
- plugin-gargoyle-usb-printer 

#### Programs
- openssl, ca-bundle, sysinfo, wifitoggle

#### Installation Guide
Open a terminal console on your PC and run ssh root@192.168.1.1 and 
respond to any prompts regarding fingerprints or passwords. Run the rest
 of these instructions in the shell you have just logged into on the 
router:
- ```scp gargoyle-1.13.0-lantiq-xway-arcadyan_arv752dpw-squashfs-sysupgrade.bin root@192.168.1.1:/tmp```
- ```sysupgrade -n -F /tmp/gargoyle-1.13.0-lantiq-xway-arcadyan_arv752dpw-squashfs-sysupgrade.bin```

Update from Luci without checking the "Keep settings" option. 

NOTE! Online package repository via Github but run first: 
- ```wget https://raw.githubusercontent.com/zuzia-dev/Easybox-802-repo-source/main/Scripts/Gargoyle_1.13/repo-fix``` 
- ```sh repo-fix```
