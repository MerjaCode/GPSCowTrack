# GPSCowTrack
Goal is to acquire GPS data from rover, cow, UAV, etc display in RT at "home" 

Goal is to acquire GPS data from rover, cow, UAV, etc display in RT at "home" via either nRF24L01 (initial effort), LoRa, WiFi, other 
This website very valuable... https://www.hackster.io/t3chflicks/smart-buoy-summary-7d1a7b
Currently, 
GPS_TAB Serial prints LAT, LONG, DATE, ZuluTime.  Capture data via Putty
nrf_muhammad-aqib_Tx and Rx work to send "High" Low" text based on a pin voltage
NEED TO DO -
0 - check transmitter_sd_smartbuy to see if it works
1 - meld GPS_TAB and nrf_muhammad-aqib_Tx into ... Tx_GPS. 
2 - Once get GPS info into "house" (computer or server), use it to create a realtime map on Google Earth or...?
3 - More from nRF24L01 to WiFi or LoRa (need to set up LORAWAN)

need these Arduino Libraries
#include <SPI.h>
#include <nRF24L01.h>
#include <RF24.h>
#include <TinyGPS++.h>
#include <SoftwareSerial.h>
#include <SD.h>
