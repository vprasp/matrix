

git clone https://github.com/rm-hull/max7219.git
cd max7219
sudo python setup.py install

sudo raspi-config
Option "A6 spi" enable

sudo apt-get install python-dev python-pip
sudo pip install max7219

connect this pins
VCC 2
GND	6
DIN 19
CS  24
CLK 23

cd ..
sudo python matrixtest.py
