# Gargoyle:1.13.X (Built 20210517-1931 git@) for Arcadyan/Astoria ARV752DPW (EasyBox 802)
[![Gargoyle](https://img.shields.io/badge/os-Gargoyle-<COLOR>.svg)](https://github.com/ericpaulbishop/gargoyle/) [![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://github.com/zuzia-dev/Easybox-904xDSL-repo-source#license) 

#### Default configuration of LAN4/TV port as WAN for cable Internet connection (not included DSL software)
- Kernel version: 4.14.232
- The router address: 192.168.1.1
- Login page: http://192.168.1.1
- SSH - Username: root 
- Password (Web & SSH): password
- WiFi is active, ssid: Gargoyle
- Password: WiFipassword

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
- Copy the image file to the router:
```scp gargoyle-1.13.0-lantiq-xway-arcadyan_arv752dpw-squashfs-sysupgrade.bin root@192.168.1.1:/tmp```

- Upload without keeping the changes with the command:
```sysupgrade -n -F /tmp/gargoyle-1.13.0-lantiq-xway-arcadyan_arv752dpw-squashfs-sysupgrade.bin```

NOTE! Update from Luci without checking the "Keep settings" option. 
