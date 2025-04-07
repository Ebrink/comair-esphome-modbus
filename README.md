# comair-esphome-modbus


This repo focusses on modbus connectivity with your Comair HRUC-Pro MVHR. As Comair and Vent-Axia are the same company, there is a chance this also works on Vent-Axia MVHR, but ymmv. Let me know if you try it.

I use a Lilygo T-CAN485 board that connects to the BMS port on the Comair MVHR (this is on the mainboard). Pinout can be found in refs/comair-pinout.png.

The modbus map can be found in refs/comair-modbus-map.pdf. Currently, I have sensors in place that pick up all values, although not all values are available (for example, the measured flow and RPM's do not report back).

Currently, I am working on integrating the User Override to be able to add CO2/Humidity sensors in HomeAssistant and then control the ventilation capacity based on those values.  
