# How to

Install [Virtualbox](https://www.virtualbox.org/wiki/Downloads)

Download the OVA file and load it in Virtualbox.

Start the machine (password is ros2)

Open VScode

Configure [platformio.ini](https://github.com/hippo5329/linorobot2_hardware/blob/master/firmware/platformio.ini) to match your ESP32/Pico device

Build the firmware and flash to your device.

Put the device in your robot car & start it

Search the network for your-robot-ip using AngryIP

Open http://your-robot-ip:8888/ in a browser and control the car

Have fun

# To be used with ESP32 cars

[Edurob](https://github.com/IDiAL-IMSL/Edurob/tree/main) not yet available for sale

[XRP Open hardware](https://www.sparkfun.com/products/22230), with encoders. No wifi transport for pico yet

[Wukong 2040](https://www.elecfreaks.com/elecfreaks-wukong2040-breakout-board-for-raspberry-pi-pico.html) no encoders

[ESP cam car](https://www.aliexpress.com/item/1005005439195049.html), no encoders

# Software installed

apt-get update

sudo apt remove unattended-upgrades

sudo apt install lubuntu-desktop thonny nemo chromium

mkdir install

cd install

wget https://raw.githubusercontent.com/linorobot/ros2me/master/install

./install

wget https://raw.githubusercontent.com/linorobot/linorobot2/humble/install_linorobot2.bash

bash install_linorobot2.bash

install https://code.visualstudio.com/

Install platformio

Install vscode extensions c/c++ & platformio manually "code --install-extension myextension.vsix

Angryip
