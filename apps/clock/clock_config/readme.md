---
parent: Harmony 3 peripheral library application examples for SAM L21 family
title: Clock configuration 
has_children: false
has_toc: false
---

[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# Clock configuration

This example application shows how to configure the clock system to run the device at maximum frequency. It also outputs a prescaled clock signal on a GPIO pin for measurement and verification.

## Description

Clock system generates and distributes the clock for the processor and peripherals. This example application shows how to use the clock manager to configure the device to run at the max possible speed. A prescaled clock signal is routed to GPIO pin to measure the frequency and accuracy of the internal device clock.

## Downloading and building the application

To clone or download this application from Github, go to the [main page of this repository](https://github.com/Microchip-MPLAB-Harmony/csp_apps_sam_l21) and then click **Clone** button to clone this repository or download as zip file.
This content can also be downloaded using content manager by following these [instructions](https://github.com/Microchip-MPLAB-Harmony/contentmanager/wiki).

Path of the application within the repository is **apps/clock/clock_config/firmware** .

To build the application, refer to the following table and open the project using its IDE.

| Project Name      | Description                                    |
| ----------------- | ---------------------------------------------- |
| sam_l21_xpro.X | MPLABX project for [SAM L21 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAML21-XPRO-B) |
|||

## Setting up the hardware

The following table shows the target hardware for the application projects.

| Project Name| Board|
|:---------|:---------:|
| sam_l21_xpro.X | [SAM L21 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAML21-XPRO-B)
|||

### Setting up [SAM L21 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAML21-XPRO-B)

- Connect an oscilloscope to monitor the PORT pin PB15 (Pin 10 of the EXT2 header)
- Connect the Debug USB port on the board to the computer using a micro USB cable

## Running the Application

1. Build and Program the application using its IDE
2. Observe a clock of 4 MHz on the clock output pin
3. LED should be blinking continuosly

Refer to the following table for clock output pin and LED name for different boards:

| Board      | Clock output pin | LED Name |
| ---------- | ---------------- |--------- |
| [SAM L21 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAML21-XPRO-B) | PB15 (Pin 10 of the EXT2 header)  | LED0 |
|||
