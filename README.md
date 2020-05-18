WaterMaster
===========

The objective is to create an automatic and *clever* system to manage the watering of my two pieces of garden (lawn + bonsai)


### Hardware
* Raspberry Pi 3
* 2 Sonoff Wi-Fi switches running the [Tasmota open source firmware](https://tasmota.github.io/docs/MQTT/)


### Software

* **Node-Red** installed as a system service on the PI
* **Mosquitto** MQTT broker, also on the PI, running as [snap package](https://snapcraft.io/) 

### Project plan

Develop a flow able to:

* Control manual operation of the two valves (Node-Red UI)
* Allow an automatic scheduling of the watering (Node-Red UI)
 
Desiderata

* In automatic mode, suspend watering if the meteorological data of the "Laste" weather station report sufficient rain. The data are freely available as part of the [OPENdata Trentino](https://dati.trentino.it/) initiative
* Allow the visualization of the data within the UI
* Add phone control/monitoring with Telegram