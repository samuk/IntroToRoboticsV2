# How to

Install [Virtualbox](https://www.virtualbox.org/wiki/Downloads)

Download the [OVA file](https://archive.org/details/ros-2_OVA_0_1)(work in progress) and load it in Virtualbox.

Start the virtual machine (password is ros2)

In the linux desktop Open VScode

Configure [platformio.ini](https://github.com/hippo5329/linorobot2_hardware/blob/master/firmware/platformio.ini) to match your ESP32/Pico device

Build the firmware and flash to your device.

Put the device in your robot car & start it

Search the network for your-robot-ip using AngryIP

Launch ROS2

Open [http://your-robot-ip:8888/](https://github.com/dheera/rosboard/pull/100) in a browser and control the car

Have fun


# BOM (WIP)

1x [XRP Open hardware](https://www.sparkfun.com/products/22230), with encoders. No wifi transport for pico yet
1x Motor holder PCB
1x [Pack of cables](https://www.aliexpress.com/item/32843338827.html)
1x [Pack of 1mm JST SH connectors](https://www.aliexpress.com/item/10000005280584.html)
4x [Bringsmart motors](https://www.aliexpress.com/item/33019382243.html)
4x [N20 wheels](https://www.aliexpress.com/item/4000099589318.html)
4x [N20 mounts](https://www.aliexpress.com/item/4000099097725.html)
1x [Battery cable](https://www.aliexpress.com/item/1005003207076823.html)
1X [9v Battery](https://www.aliexpress.com/item/1005005523610603.html)

# Other PicoW or ESP32 cars may work too

[Edurob](https://github.com/IDiAL-IMSL/Edurob/tree/main) not yet available for sale

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

git config --system core.longpaths true

Angryip

[Rosboard fork](https://github.com/dheera/rosboard/pull/100)
