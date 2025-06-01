LoRa Chat Project
Overview
This repository contains the Arduino code and documentation for our group's LoRa communication experiment conducted as part of Assignment 003: Experimenting with LoRa. The goal of the experiment was to test the range and reliability of LoRa communication using LoRa32u4 II (BSFrance) modules, with one group acting as a stationary base station and the other as a mobile node. The experiment was conducted on May 30, 2025 [REPLACE WITH YOUR EXPERIMENT DATE], and we successfully communicated at a distance of 500 meters [REPLACE WITH YOUR DISTANCE] at the coordinates 40.7128, -74.0060 [REPLACE WITH YOUR COORDINATES].
Hardware Requirements

LoRa32u4 II (BSFrance): Two modules, one for the sender and one for the receiver.
Antenna: Compatible with 915 MHz [REPLACE WITH YOUR REGION’S FREQUENCY, e.g., 868 MHz for Europe].
USB Cable: For programming and powering the LoRa32u4 II modules.
Computer: With Arduino IDE installed for uploading code.
Optional: Battery pack for mobile node testing in the field.

Software Requirements

Arduino IDE: Version 2.3.2 or later.
Adafruit AVR Boards: Install via Arduino IDE Boards Manager using the URL https://adafruit.github.io/arduino-board-index/package_adafruit_index.json.
RadioHead Library: Install via Arduino IDE Library Manager (search for "RadioHead").
Git: For cloning and pushing to this repository.

Setup Instructions

Install Arduino IDE:
Download and install from arduino.cc.


Add Board Support:
In Arduino IDE, go to File > Preferences.
Add https://adafruit.github.io/arduino-board-index/package_adafruit_index.json to Additional Boards Manager URLs.
Go to Tools > Board > Boards Manager, search for "Adafruit AVR Boards," and install.


Install RadioHead Library:
In Arduino IDE, go to Sketch > Include Library > Manage Libraries.
Search for "RadioHead" and install.


Connect Hardware:
Connect the LoRa32u4 II module to your computer via USB.
Attach the antenna to ensure proper signal transmission.


Upload Code:
Open sender.ino and receiver.ino from this repository in the Arduino IDE.
Select Tools > Board > Adafruit Feather 32u4.
Set the frequency to 915.0 [REPLACE WITH YOUR REGION’S FREQUENCY, e.g., 868.0 for Europe] in both sketches.
Upload sender.ino to one module and receiver.ino to the other.


Test Communication:
Power both modules.
Open the Serial Monitor (Tools > Serial Monitor, 9600 baud) to view messages on the receiver.
Move the mobile node (sender) to test the communication range.



Project Structure

sender.ino: Arduino sketch for the LoRa sender (mobile node).
receiver.ino: Arduino sketch for the LoRa receiver (base station).
README.md: This file, documenting the project.

Experiment Details

Objective: Test the range of LoRa communication between two LoRa32u4 II modules.
Setup: One group remained stationary at 40.7128, -74.0060 [REPLACE WITH BASE STATION COORDINATES], acting as the receiver (base station). The other group moved with the sender to test the maximum communication range.
Final Successful Communication:
Coordinates: 40.7128, -74.0060 [REPLACE WITH MOBILE NODE COORDINATES FROM GOOGLE MAPS]
Distance: 500 meters [REPLACE WITH DISTANCE MEASURED USING GOOGLE MAPS]


Frequency Used: 915 MHz [REPLACE WITH YOUR FREQUENCY, e.g., 868 MHz for Europe].
Environment: Urban setting with buildings and trees as obstacles [REPLACE WITH YOUR ENVIRONMENT DESCRIPTION, e.g., rural, campus].

Usage

Run the Receiver:
Upload receiver.ino to the stationary LoRa32u4 II module.
Open the Serial Monitor to view incoming messages.


Run the Sender:
Upload sender.ino to the mobile LoRa32u4 II module.
The sender transmits "Hello LoRa!" every 5 seconds.


Measure Range:
Move the sender away from the receiver while monitoring the Serial Monitor.
Record the final location and distance where communication is successful using Google Maps’ “Measure Distance” feature (right-click > Measure Distance).


Analyze Results:
Document the coordinates and distance of the last successful communication point.



Contributors

Wilson Bugiri (bugiriwilson651) [REPLACE WITH YOUR GITHUB USERNAME]
Group Member 1 ([username1]) [REPLACE WITH NAME AND GITHUB USERNAME]
Group Member 2 ([username2]) [REPLACE WITH NAME AND GITHUB USERNAME]

License
This project is licensed under the MIT License. See the LICENSE file for details.
Acknowledgments

Thanks to our instructor and group members for their support during the experiment.
RadioHead library by Mike McCauley for simplifying LoRa communication.
Adafruit for providing board support for the LoRa32u4 II.

