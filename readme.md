# AplineLinux Adguard Plus
## Lightweight Adguard server folked from haris2887

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

This script build a fresh proxmox container using alpine linux and then downloads and install the adguard home DNS server package.
It is extreamlight weight container that runs on minimal resources

NB: haris2887's script didnt work for me, because my local storage can not install lxc containers. Therefore, I added option to specify storage during setup. The service keeps stoping, so i added code to restart it if it stops. And updated alpine version to 3.17

## How To Run
- You must run the below commands as root user
1. su - root
2. curl -LJO https://raw.githubusercontent.com/kjames2001/Adguardd-Proxomx/private/install.sh && chmod +x install.sh &&./install.sh && rm install.sh
