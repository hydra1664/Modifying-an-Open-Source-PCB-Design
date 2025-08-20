# Arduino Nano USB-C Modification

## Overview
This project is a reverse-engineered and modified version of an open-source Arduino Nano clone.  
The idea was to explore PCB design changes in KiCad, upgrade the board to modern standards, and document the process.  

## Base Design
- Board chosen: Arduino Nano clone from KiCad’s open-source library  
- Why this board?  
  - Simple but widely used in prototyping and embedded projects  
  - Compact design with just enough complexity for meaningful modifications  
  - A great test case for experimenting with USB connector upgrades  

## Modifications
### 1. USB-C Connector Upgrade
- Replaced the legacy Micro-USB port with a USB-C connector  
- Chose a compact footprint that fit the Nano’s small PCB without major rerouting  
- Makes the board more user-friendly and future-proof  

### 2. Added 5.1kΩ Pull-Down Resistors
- Two 5.1kΩ resistors added on CC1 and CC2 pins  
- Ensures proper USB-C configuration and reliable detection  

### 3. Improved Routing with Vias
- Added multiple ground and signal vias near the USB-C connector  
- Helps maintain clean return paths and improves signal integrity  

## Verification
- Ran KiCad’s Design Rule Check (DRC) after modifications  
- No clearance, spacing, or connectivity issues were found  

## Images
The repository includes images showing the original and modified design:

- Original_DRC.png
- <img width="1920" height="1080" alt="Original_DRC" src="https://github.com/user-attachments/assets/8f64a217-4b9a-4515-a52e-8d8ec1ed17bc" />
- Modified_DRC.png
- Original_Schematics.png
- Modified_Schematics.png 
- Zoomed_Original_Schematics.png  
- Zoomed_Modified_Schematics.png  

## Project Files
- Modified KiCad project files  
- Before/after schematics and DRC results  
- Screenshots for visual comparison  

## Tools Used
- KiCad (open-source EDA tool)  

## Learnings
- How to properly select and fit a USB-C footprint on a compact board  
- The importance of routing discipline and signal return paths  
- Making small but meaningful hardware improvements that modernize older designs  

Author: Mohammad Amash  
Date: May 2025  
