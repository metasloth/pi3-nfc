# pi3-nfc
A codebase for testing out using an NFC RFID sensor with a Raspberry Pi 3

## Basic
https://www.raspberrypi.org/downloads/raspbian/
username: pi
password: raspberry

sudo raspi-config

### Keyboard

https://www.raspberrypi.org/forums/viewtopic.php?t=9136
sudo dpkg-reconfigure keyboard-configuration
select English(US)
reboot


## Wifi
sudo iwlist wlan0 scan
sudo nano /etc/wpa_supplicant/wpa_supplicant.conf
append 
network={
    ssid="testing"
    psk="testingPassword"
}
reboot


### ssh
sudo raspi-config


### node
curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
sudo apt-get install -y nodejs

