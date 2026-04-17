# Satellite Image Receiving Station
**Developed by [Dhairya Khanna](https://github.com/YOUR_GITHUB_USERNAME)**

This repository contains the CAD models, designs, and technical documentation for a DIY satellite image receiving station.

## Overview
This project is designed to track and receive signals from polar-orbiting satellites (such as NOAA and Meteor-M series) to decode real-time weather imagery.

## How It Works

### 1. The Antenna (QFH)
The system uses a **Quadrifilar Helix (QFH)** antenna. This antenna is specifically designed for satellite reception because it handles circular polarization and has a wide "field of view," meaning it can catch signals as soon as a satellite rises above the horizon.

![QFH Antenna](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRyP19eOPSxOWqbYZEkPNndTB2eufk0QGnT_g&s)
*Note: Image for reference. Physical build currently in progress.*

### 2. The Receiver (RTL-SDR v4)
The signals are sent from the antenna to an **RTL-SDR v4**. 
* **Hardware Choice:** The v4 is the recommended choice for this project due to its improved filtering and performance over the v3, despite being nearly the same price.

![RTL-SDR v4](https://www.wimo.com/media/catalog/product/cache/b841b4d4ee9f74003d622bd3123ed748/R/T/RTL_SDRV4_stick_sma_e535.jpg)

### 3. Signal Capture & Software
The radio signals are processed through software such as **SatDump**. The software displays a "Waterfall," which is a visual representation of the signal intensity over time as the satellite passes over.

![Signal Waterfall](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRD6jL9KgbcjaejfZa2o9zzOjtIIPvAmlFbjQ&s)
*Example of the signal waterfall captured during a pass.*

### 4. Image Decryption
The final step is decrypting the captured signal into a usable image. Below is an example of the type of imagery captured from NOAA satellites.

![NOAA Satellite Image Example](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRiPXeU6pjg2EfojMu8Z_feOOOtfhPuPZ1iLA&s)
