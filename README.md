# LoRa Chat Project

## Overview

This repository contains the Arduino code and documentation for our group's **LoRa communication experiment** conducted as part of Assignment **003: Experimenting with LoRa**. The goal of the experiment was to test the range and reliability of LoRa communication using LoRa32u4  modules, with one group acting as a stationary base station and the other as a mobile node.

- **Experiment Date:** May 29, 2025 
- **Communication Distance:** 71.81 meters
- **Coordinates:**  -1.6018040425775748, 29.51636611011121

## Hardware Requirements

- **LoRa32u4 :** Two modules (one for sender and one for receiver)
- **Antenna:** Compatible with 915 MHz
- **USB Cable:** For programming and powering the modules
- **Computer:** With Arduino IDE installed

## Software Requirements

- **Arduino IDE:** Version 2.3.2 or later
- **Adafruit AVR Boards:**  
  Install via Arduino IDE Boards Manager using the URL:  
  `https://adafruit.github.io/arduino-board-index/package_adafruit_index.json`
- **RadioHead Library:**  
  Install via Arduino IDE Library Manager (search for "RadioHead")
- **Git:** For cloning and pushing to this repository

## Setup Instructions

### 1. Install Arduino IDE

Download and install the Arduino IDE from [arduino.cc](https://www.arduino.cc).

### 2. Add Board Support

1. Open Arduino IDE and navigate to **File > Preferences**.
2. Add the following URL to **Additional Boards Manager URLs**:  
   `https://adafruit.github.io/arduino-board-index/package_adafruit_index.json`
3. Go to **Tools > Board > Boards Manager**, search for **"Adafruit AVR Boards"**, and install.

### 3. Install RadioHead Library

1. In Arduino IDE, go to **Sketch > Include Library > Manage Libraries**.
2. Search for **"RadioHead"** and install.

### 4. Connect Hardware

- Connect the LoRa32u4 II module to your computer via USB.
- Attach the antenna to ensure proper signal transmission.

### 5. Upload Code

- Open **lora_chat.ino**  in the Arduino IDE.
- Select **Tools > Board > Adafruit Feather 32u4**.
- Set the frequency to `915.0`

### 6. Test Communication

- **Power Both Modules:** Power on the sender and receiver.
- **Monitor Serial Output:** Use Serial Monitor from **Tools > Serial Monitor** at **115200 baud** to view messages.
- **Experiment:** Move the mobile node (sender) to test the communication range.

## Project Structure

- **lora_chat.ino:** Arduino sketch for the LoRa chatting
- **README.md:** This documentation file

## Experiment Details

- **Objective:** Test the range of LoRa communication between two modules
- **Setup:**  
  - The receiver (base station) remained stationary at 40.7128, -74.0060 
  - The sender (mobile node) was moved to test the maximum communication range.
- **Final Successful Communication:**  
  - **Coordinates:**  -1.6018040425775748, 29.51636611011121
  - **Distance:** 72.81

- **Frequency Used:** 915 MHz 
- **Environment:** Urban setting with buildings and trees as obstacles 

## Usage

### Run the Receiver

1. Upload **lora_chat.ino** to the stationary LoRa32u4 II module.
2. Open the Serial Monitor to view incoming messages.


### Measure Range

- Move the sender away from the receiver while monitoring the Serial Monitor.
- Record the final location and distance using Google Maps’ “Measure Distance” feature (right-click > Measure Distance).

### Analyze Results

- Document the coordinates and distance of the last successful communication point.

## Contributors
- **BUGIRI Wilson Goal** ([GitHub](https://github.com/goal651))



