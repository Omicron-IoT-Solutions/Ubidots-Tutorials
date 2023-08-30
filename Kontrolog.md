# Connect your Kontrolog devices over LoRaWAN to Ubidots
*Learn how to connect your Kontrolog devices to Ubidots through TTN, to remotely monitor sensor readings, output status, perform remote control, and send configuration messages to the device.*

## Introduction
The Kontrolog device is a programmable controller for IoT (Internet of Things), designed for remote and real-time control and monitoring of different processes with high security and precision requirements. It can be connected to a touch screen HMI for local visualization and configuration. Adapted to your application, the device can be easily used after installation.

Kontrolog devices have a dual communication module Sigfox/LoRaWAN™ that allows them to send data to the Ubidots platform through either of these two networks, giving it a plus in different application fields, such as industry, agriculture, water quality, home automation, among others.

It includes five (5) Analog/Digital inputs for sensors, one (1) analog input for battery sensor from 0 to 12 VDC, one (1) AC voltage sensor input [0 to 250 VAC], one (1) input to measure AC current in the ranges of 0-30 A, 0-50 A, 0-100 A, one Modbus (RS-485) input port operating as a master on the network, and five (5) control outputs (Relay-type, and analog output, depending on the model of the device ordered). For further information visit the website. 

Following this guide, the user will be able to connect the Kontrolog to Ubidots, using The Things Network (TTN). From there, the users will be able to perform, among other things:
+ Remote monitoring and visualization of current measurements, state of the outputs and sensor’s variable records, in graphs and data tables, for up to 2 years.
+ Remote configuration of the device parameters.
+ Alarm management for variables out of range, battery levels, and AC power failure.
+ Set alarm limits, alarm events, and notifications via email, SMS, voicemail, Telegram messaging service, or webhooks.

## Requirements
+ Kontrolog
+ The Things Network (TTN) account
+ Ubidots account with the UbiFunctions add-on enabled

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

