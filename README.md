# Demo of WT32-SC01 ESP32 display with openHASP, Philips HUE, MQTT and node-RED
Display module: wireless-tag [WT32-SC01](https://www.seeedstudio.com/ESP32-Development-board-WT32-SC01-p-4735.html) (3.5" 320x480 capacitive multi-touch screen) ESP32 Development board.

# Demo
[![Demo](https://img.youtube.com/vi/U9RnkEKp-HY/0.jpg)](https://www.youtube.com/watch?v=vptJk92lRF4&list=PLFmnthuksGmyfad69c77FCcRjeLGO3adU)

# 3d printed case
![](./assets/printminion-WallmountCase-Solid-WT32-SC01.jpg)
![](./assets/printminion-WallmountCase-Door-WT32-SC01.jpg)
![](./assets/printminion-DesktopCase-Portrait-WT32-SC01.jpg)
![](./assets/printminion-DesktopCase-Landscape-WT32-SC01.jpg)

* on [cults3d](https://cults3d.com/en/users/printminion/creations)
* on [shapeways](https://www.shapeways.com/shops/printminion)
* follow me on Twitter [@printminion](https://twitter.com/printminion)

# Setup

## Setup WT32-SC01 with openHASP
* openHASP
https://openhasp.haswitchplate.com/0.6.1/devices/wt32-sc01/
* flash esp32
https://openhasp.haswitchplate.com/0.6.1/installation/esp32/

* edit config
  * open url
  * open file [config.json](./plate/config.json)
  * set WIFI
  * add MQTT server
* edit interface files
  * [offline.cmd](./plate/offline.cmd)
  * [online.cmd](./plate/offline.cmd)
  * [pages.jsonl](./plate/pages.jsonl)

![page 1](./docs/plate01/plate01-page_1.jpg)
![page 2](./docs/plate01/plate01-page_2.jpg)
![page 3](./docs/plate01/plate01-page_3.jpg)
![page 4](./docs/plate01/plate01-page_4.jpg)

* you can change screen rotation to 90°
* reboot
* check page #5

![page 5](./docs/plate01/plate01-page_5.jpg)

## Setup MQTT on Node-Red
* install node-red on raspberry pi
* install mqtt server
* use the flow (coming soon) to use the plate with mqtt server
![mqtt flow](./docs/node-red/Node-RED-hue-flow.png)