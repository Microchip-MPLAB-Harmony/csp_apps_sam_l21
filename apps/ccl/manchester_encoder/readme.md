---
parent: Harmony 3 peripheral library application examples for SAM L21 family
title: CCL Manchester Encoder 
has_children: false
has_toc: false
---

[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# CCL Manchester Encoder

This example application shows how to use the CCL peripheral library and generate a Manchester-encoded output.

## Description

This demonstrates a way to generate a Manchester-encoded output using a SPI port and the CCL. The SPI port is sending out a predefined buffer of data in a circular fashion. Data is sent out LSB first, with CCL_OUT being the Manchester-encoded output. Pins are configured such that a logic analyzer can be attached to see the input (MOSI and SCK) and the output (CCL_OUT) simultaneously.

## Downloading and building the application

To clone or download this application from Github, go to the [main page of this repository](https://github.com/Microchip-MPLAB-Harmony/csp_apps_sam_l21) and then click **Clone** button to clone this repository or download as zip file.
This content can also be downloaded using content manager by following these [instructions](https://github.com/Microchip-MPLAB-Harmony/contentmanager/wiki).

Path of the application within the repository is **apps/ccl/manchester_encoder/firmware** .

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

- Use jumper from PA09 (EXT1 pin 12) to PB01 (EXT3 pin 4). This routes SCK to CCL_IN[2]
- PA08 (EXT1 pin 11) has MOSI output
- PA07 (EXT1 pin 18) has CCL output (CCL_OUT)
- Connect the Debug USB port on the board to the computer using a micro USB cable

## Running the Application

1. Connect a logic analyzer to MOSI pin
2. Connect a logic analyzer to SCK pin
3. Connect a logic analyzer to the Manchester-encoded output CCL_OUT pin
4. Refer to the following table for pin details:
    |Board| MOSI pin | SCK pin  | CCL_OUT pin |
    |-----|----------|----------|-------------|
    |[SAM L21 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAML21-XPRO-B)| PA09 (EXT1 pin 12) | PA08 (EXT1 pin 11) | PA07 (EXT1 pin 18) |
    ||||

5. Build and Program the application using its IDE
6. Observe the output on logic analyzer, it should follow the truth table as shown in the following diagram:

    ![output](images/truth_table_manchester_encoder.png)
