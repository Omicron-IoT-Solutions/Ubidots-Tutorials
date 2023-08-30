# Connect your Kontrolog devices over LoRaWAN™ to Ubidots
*Learn how to connect your Kontrolog devices to Ubidots through TTN, to remotely monitor sensor readings, output status, perform remote control, and send configuration messages to the device.*

## Requirements
+ [Kontrolog](https://omicroniot.com/beta-9-2/)
+ The Things Network (TTN) account
+ [Ubidots account](https://es.ubidots.com/signup) with the [UbiFunctions add-on enabled](https://help.ubidots.com/en/articles/2094690-plans-billing-how-to-add-ubifunctions-to-my-account)

## Step-by-Step
1. Uplink function to post data to Ubidots   
   1.1. Create UbiFunction for Uplink messages   
   1.2. Communications protocol for Uplink messages   
2. Downlink function to get data from Ubidots   
   2.1. Create UbiFunction for Downlink messages   
   2.2. Communications protocol for Downlink messages   
   2.3. Create a generic dashboard to send Downlink messages   
3. Setting up TTN   
   3.1. Callback configuration for LoRaWAN™ Uplink Messages   
   3.2. Downlink API Key   
   3.3. Format for Uplink payload   
4. Setting up the Kontrolog

## 1. Uplink function to post data to Ubidots
Below is the schematic representation of how information travels from a Kontrolog device to the Ubidots platform through the LoRaWAN™ network:

