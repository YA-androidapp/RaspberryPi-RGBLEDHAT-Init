# RaspberryPi-RGBLEDHAT-Init

---

```bash
sudo apt update -y && sudo apt upgrade

sudo apt-get install build-essential python-dev scons swig
sudo apt install python3-pip
sudo apt install python3-bottle

sudo python3 -m pip install rpi_ws281x
sudo python3 -m pip install neopixel


cd ~
wget -O rpi_ws281x-master.zip https://github.com/jgarff/rpi_ws281x/archive/refs/heads/master.zip
unzip rpi_ws281x-master.zip
cd rpi_ws281x-master/
sudo scons
sudo ./test

cd ~
wget -O rpi-ws281x-python-master.zip https://github.com/rpi-ws281x/rpi-ws281x-python/archive/refs/heads/master.zip
unzip rpi-ws281x-python-master.zip
cd rpi-ws281x-python-master/examples/
python3 strandtest.py

cd ~
wget https://www.waveshare.com/w/upload/a/ae/RGB_LED_HAT.tar.gz
tar -zxvf RGB_LED_HAT.tar.gz
cd RGB_LED_HAT/web-RGB/
python3 main.py
```
