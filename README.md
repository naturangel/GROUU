# NEXT TASKS (delete after done)

1. finish documentation (day3.pdf) on who to build a mainSoilProbe with a nodeMCU;

Day3 Afternoon: solder workshop







# JOURNAL


## configuring Raspberry Pi zero W as server

#### configuring the Pi
https://core-electronics.com.au/tutorials/raspberry-pi-zerow-headless-wifi-setup.html

#### Accessing through ssh on mac or linux terminal
https://www.raspberrypi.org/documentation/remote-access/ssh/unix.md

#### upgrade Node-Red and Node.js
1. open terminal;
2. commands:
```
sudo apt-get update
sudo apt-get upgrade
bash <(curl -sL https:/raw.githubusercontent.com/node-red/raspbian-deb-package/master/resources/update-nodejs-and-nodered)
sudo systemctl enable nodered.service
```
3. Connect to Raspberry Pi Node-red console throught your browser be accessing ```http://"raspipaddress":1880```

4. Install Mosquitto MQTT broker
```sudo apt-get install Mosquitto```

some instructions on how to test here: https://www.instructables.com/id/Installing-MQTT-BrokerMosquitto-on-Raspberry-Pi/

##### other useful links:
Security: manage permissions on node-red tutorial - https://www.youtube.com/watch?v=GeN7g4bdHiM


## mainSoilProbe REV0

### pin list:

DHT pin


### This board includes:
DHT22 (Humidity and Temperature - Near plants Control);
1 x 3 male header for DS18B20 (encapsulated version for Soil Temperature);
2 x 2 male header connections for Moisture 10k with Two probes (one for each probe requiring calibration - see calib. instructions);
1 led (no usage yet, mostly for debug purposes);
1 ftdi set headers;
1 voltage converter 12V - 3,3V;
1 x 2 screw headers to add solar panel + battery (maybe connect solar battery pack now).

### refs:
#### solarpower
https://www.aki.pt/electricidade/producao-energia-renovavel/solar-eolico-energia-propia/acessorios-de-energias-renovaveis/bateria/controladores/painelmanutencaobaterias-p10533.aspx#info
https://www.aki.pt/electricidade/producao-energia-renovavel/solar-eolico-energia-propia/kits-solares/kitbombadeaguamicrosolar-p49581.aspx
https://mauser.pt/catalog/product_info.php?products_id=82391

Main Probe

#### Multiple Analogs -

https://www.instructables.com/id/Multiple-Analog-Inputs-on-Only-One-Analoge-Pin/

#### ESP12 + DHT22 -

https://cityos.io/tutorial/2006/ESP12-and-DHT22

#### ESP12  + temp

https://iot-playground.com/blog/2-uncategorised/41-esp8266-ds18b20-temperature-sensor-arduino-ide

#### Voltage Regulator

http://www.ti.com/lit/ds/symlink/lm3480.pdf

#### use FTDI on ESP12

https://www.hackster.io/harshmangukiya/program-esp8266-esp-12e-with-arduino-using-ftdi-cable-2310c9


### refs fabrication:
#### eagle to flatCAM

http://caram.cl/software/flatcam/board-cutout-with-flatcam/
