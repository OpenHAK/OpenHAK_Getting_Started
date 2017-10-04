# GETTING STARTED WITH OPENHAK
Kit contents:
  1. OpenHAK board
  2. Battery
  3. Wrist strap
  4. Breakout Connector - for HAKing ;)
  5. Rubber tube

##Setup Your Kit:
- Download the OpenHAK app - links to come
- Attach the strap to side of you OpenHAK board with the battery connector
- Connect the Battery
- Slide rubber tube over strap and battery
- Put it on!
- Connect it to the app to sync the current time/date
- Live

##Default App:
The app pre-flashed on the kit does the following
Every Ten minutes (if connected to the app or not)
- Captures 30 seconds of heart-rate data. The median value as well as the standard deviation from these captures values are saved
- Records the total number of steps taken
- Saves this data along with the timestamp for comparison later
- The board will retain approximatly three days worth of data at this ten minute interval

The data can be synced to the app at any time and viewed in graph form.

## OpenHAK Board:
The OpenHAK board is based on the Simblee BLE module. This module supports the Arduino platform and also supports over-the-air (OTA) firmware uploading. (See HAKing section for more details)

The sensors on the OpenHAK board are the MAX30102 optical PPG/SpO2, and the BMP160 6-axis IMU.
