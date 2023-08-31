
 ![Bot](https://raw.githubusercontent.com/samuk/IntroToRoboticsV2/main/course/ros2/bot.jpg)
# BOM (WIP)

1x [XRP Open hardware](https://www.sparkfun.com/products/22230), with encoders. No wifi transport for pico yet. Could be used with [open hardware pico](https://www.olimex.com/Products/MicroPython/RP2040-PICO30/open-source-hardware)

1x [Motor holder PCB](https://easyeda.com/editor#id=e655b08f80cd412e8119d61893779e39) (just register and one click order from JLPCB)

1x [1mm > 1mm Pack of cables](https://s.click.aliexpress.com/e/_De5zhCP)

1x [Pack of 1mm JST SH connectors](https://s.click.aliexpress.com/e/_DDIr1m7)

4x [6v 150RPM Bringsmart motors](https://s.click.aliexpress.com/e/_DC72ruf)

4x [N20 wheels](https://s.click.aliexpress.com/e/_DBjDZqx)

4x [N20 mounts](https://s.click.aliexpress.com/e/_Dm7LWRD)

1x pack [18mm female standoffs](https://www.aliexpress.com/item/32539100523.html)

1x pack [M3 x 6mm screw](https://www.aliexpress.com/item/32539100523.html)

1x [Battery cable](https://www.aliexpress.com/item/1005003207076823.html)

1X [9v Battery](https://s.click.aliexpress.com/e/_DdPChq3)

Or alternately a upgraded [Fatshark battery pack](https://www.amazon.co.uk/Tattu-2500-mAh-Replacement-Battery-Fatshark/dp/B071D92NWW) or [18650 battery](https://s.click.aliexpress.com/e/_DClgys7) or open hardware [18650 battery](https://oshwlab.com/wagiminator/fp6277-power-bank)

# How to

Install [Virtualbox](https://www.virtualbox.org/wiki/Downloads)

Download the [OVA file](https://archive.org/details/ros-2_OVA_0_1) (work in progress) and load it in Virtualbox. ~6Gb ~5hr download.

Start the virtual machine (password is ros2)

In the linux desktop Open VScode

If using a ESP3 configure [platformio.ini](https://github.com/rosmo-robot/linorobot2_hardware_ESP32_Pico/blob/master/firmware/platformio.ini) to match, defaults to PicoW.

Build the firmware and flash to your device.

Put the device in your robot car & start it

Search the network for your-robot-ip using AngryIP

Launch ROS2

Open [http://your-robot-ip:8888/](https://github.com/dheera/rosboard/pull/100) in a browser and control the car

Have fun

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
