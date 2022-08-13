# sendDataOverMQTT
Raw sensors datalogging functionality using Bosch XDK110.
Starting from XDK workbench IDE tool, i writed an application that send all sensors data in json format to MQTT broker over WI-FI.

# DISCLAIMER
After reading this, download the `zip` file, over the Releases page, import into your XDK Workbench, compile and flash the project on the XDK.

## Brief description
XDK Datalogger logs sensor data to a file in the SD Card. The output file is `data_##.csv`.

## Sensors enabled
- Accelerometer [mG]
- Humidity [%]
- Pressure [hPa]
- Temperature [C]
- Light intensity [Lm]

## Requirements
- [XDK Workbench](https://developer.bosch.com/web/xdk/downloads)
- WI-Fi connection
- A broker MQTT

## Features
- No more complete file overwrite on reboot. A new file it's created for each session.
- File count index retention on a second file named "index.xdk", stops files getting overwrited on reboot.
- No known file size limit for a session.
