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
