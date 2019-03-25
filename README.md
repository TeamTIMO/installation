# Installation

Software to be installed.

## mqtt

- `curl -O http://repo.mosquitto.org/debian/mosquitto-repo.gpg.key'
- `sudo apt-key add mosquitto-repo.gpg.key'
- `rm mosquitto-repo.gpg.key'
- `cd /etc/apt/sources.list.d/'
- `sudo curl -O http://repo.mosquitto.org/debian/mosquitto-jessie.list'
- `sudo apt-get update'
- `sudo apt-get install mosquitto mosquitto-clients'

(Source: https://hackaday.com/2016/05/09/minimal-mqtt-building-a-broker/)

## node.js

- `sudo apt remove nodered -y`
- `sudo apt remove node nodejs nodejs-legacy -y`
- `sudo apt remove npm -y`
- `sudo apt remove --purge node`
- `curl -sL http://deb.nodesource.com/setup_10.x | sudo bash -`
- `sudo apt-get install nodejs`

## pm2

`npm install pm2 -g`

## nginx

`sudo apt-get install nginx`

## festival

`sudo apt-get install festival festvox-kallpc16k`

## omxplayer

`sudo apt-get install omxplayer`

## timo-scan

- `cd /opt`
- `git clone https://github.com/TeamTIMO/timo-scan.git .`
- `cd timo-scan`
- `npm install`
- `mv config.sample.json config.json`
- `pm2 start index.js --name '0000_timo-scan'`

## timo-tts

- `cd /opt`
- `git clone https://github.com/TeamTIMO/timo-tts.git .`
- `cd timo-tts`
- `npm install`
- `mv config.sample.json config.json`
- `pm2 start index.js --name '0000_timo-tts'`

## timo-mp3

- `cd /opt`
- `git clone https://github.com/TeamTIMO/timo-mp3.git .`
- `cd timo-mp3`
- `npm install`
- `mv config.sample.json config.json`
- `pm2 start index.js --name '0000_timo-mp3'`