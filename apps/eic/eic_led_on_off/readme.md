---
parent: Harmony 3 peripheral library application examples for SAM L21 family
title: EIC Interrupt 
has_children: false
has_toc: false
---

[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# EIC Interrupt

This example application demonstrates how to generate interrupt using the EIC on switch press and indicate it through an LED.

## Description

The application registers an event callback with EIC Peripheral library and toggles an LED for every switch press event.

## Downloading and building the application

To clone or download this application from Github, go to the [main page of this repository](https://github.com/Microchip-MPLAB-Harmony/csp_apps_sam_l21) and then click **Clone** button to clone this repository or download as zip file.
This content can also be downloaded using content manager by following these [instructions](https://github.com/Microchip-MPLAB-Harmony/contentmanager/wiki).

Path of the application within the repository is **apps/eic/eic_led_on_off/firmware** .

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

- Connect the Debug USB port on the board to the computer using a micro USB cable

## Running the Application

1. Build and Program the application using its IDE
2. LED toggles on every switch release

Following table provides the Switch and LED name:

| Board      | Switch Name | LED Name |
| ---------- | ---------| ------------|
| [SAM L21 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAML21-XPRO-B) | SW0 | LED0 |
||||
