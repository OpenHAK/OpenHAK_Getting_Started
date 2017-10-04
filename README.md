# GETTING STARTED WITH OPENHAK
Kit contents:
  1. OpenHAK board
  2. Battery
  3. Wrist strap
  4. Breakout Connector - for HAKing ;)
  5. Rubber tube

##Setup Your Kit:
- Download the OpenHAK app - [Android](https://github.com/OpenHAK/ohak_android)  - iOS (App pending review)
- Attach the strap to battery connector side of you OpenHAK board
- Connect the Battery (Should blink Red,Green,Blue)
[![Startup](https://img.youtube.com/vi/IthpAmcseeE/0.jpg)](http://www.youtube.com/watch?v=IthpAmcseeE)

- Slide rubber tube over strap and battery
- Put it on!
- Connect it to the app to sync the current time/date
- Live

## OpenHAK Board:
The OpenHAK board is based on the Simblee BLE module. This module supports the Arduino platform and also supports over-the-air (OTA) firmware uploading. (See HAKing section for more details)

Included on the OpenHAK board are the MAX30102 optical PPG/SpO2 sensor, and the BMP160 6-axis IMU, li-po battery charger via USB, and a breakout connector to be able to add on hardware and HAK your device.

###Default Firmware:

[Repo Here](https://github.com/OpenHAK/OHAK_firmware)

The app pre-flashed on the kit does the following
Every Ten minutes (if connected to the app or not)
- Captures 30 seconds of heart-rate data. The median value as well as the standard deviation from these captures values are saved
- Records the total number of steps taken
- Saves this data along with the timestamp for comparison later
- The board will retain approximatly three days worth of data at this ten minute interval. After 512 samples are recorded, the oldest samples are removed.

The data can be synced to the app at any time and viewed in graph form.

##OpenHAK Mobile Apps:
The mobile apps provided with the OpenHAK platform are identical, and were created using Evothings/Cordova.

[Repo Here](https://github.com/OpenHAK/openhak_evothings)

###Current Features:
- Scan for available OpenHAKs: All nearby OpenHAKs, not connected to an app, will show up with their unique device IDs.
- Connect to an OpenHAK: Clicking the OpenHAK ID will initiate the BLE connection, automatically sync the current time/data, and download all the stored samples on the device.
- Download History data: If you leave the app connected to the device, this will sync all available data from the device to the phone, and show the data on the graph.
- Disconnect the device: The device will capture data even while disconnected, so don't be scared.
- Debug Info: These text areas show the last packet of data received from the device, as well as the total number of packets that were sent during a history transfer

####Coming Soon
- [ ] Save device and auto connect
- [ ] Store history data on phone, and download/share data
- [ ] Better graphing and data visualization
- [ ] Trigger realtime heart-rate caputure
