# Connect your belgian counter to Home Assistant with ESPhome
Use a Wemos ESP32-C3 Pico to read data from P1 port of your belgian electricity counter with ESPhome

# Hardware
This project requires a Wemos ESP32 C3 Pico, a flat RJ12 cable and a 3D printer if you want to print the case (which requires 2 M2x10 screws)

Here is the links to buy the required material :

- Wemos ESP32-C3 Pico : https://fr.aliexpress.com/item/1005004866531117.html
- Flat RJ12 cable : https://s.click.aliexpress.com/e/_DC5f42T
- M2x10 stainless screws : https://s.click.aliexpress.com/e/_Dmchbtl
- You can find the 3D models of the case here : https://makerworld.com/en/models/502472#profileId-417722

> Note : I will maybe work on a variant using ESP32 C6 as it is more future proof (supports WiFi 6) and generally cheaper

You can find the full video guide here :

[![ESP32 Pico for Belgian electricity counter](https://img.youtube.com/vi/KM2kO0HSWFs/hqdefault.jpg)](https://youtu.be/KM2kO0HSWFs)

# Wiring
![RJ12-pins](https://github.com/tomsbasement/esp32-pico-p1/assets/108102/e30a5d2b-0883-4c2d-89bc-5bb175bf30bc)

<img src="https://github.com/tomsbasement/esp32-pico-p1/assets/108102/4ab4b4a1-7a0a-4ccf-bf76-ba80f823f1ae" alt="ESP32-C3 wiring" width="410"/>

# Instructions
This project uses esphome-p1mini project as external component for esphome : https://github.com/Beaky2000/esphome-p1mini

1. Install ESPhome
2. Go yo your ESPhome dashboard with Chrome or any other browser that supports Webserial
3. Plug your ESP32 to your computer while pressing the "boot" button on your ESP32
4. Release the boot button
5. On your ESPhome dashboard, click on "New device", on the bottom right
6. Follow the instructions to add install ESPhome on your device
7. Call it whatever you want, by default, this project uses "Compteur Ores"
8. Once the device is ready, copy the yaml of this project and adapt the variables to the ones provided in your own project file
9. Install the new configuration
10. Plug your device to your P1 port, if it turns on and the light is blue, you are ready to receive data on your Home Assistant installation !

Video instructions (in French) :
To be done
