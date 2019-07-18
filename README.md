# water-meter-measurement-system
This is an overview of different project part to digitalize an analog water meter and use it for a house automatization system to controll the water consumption.

# Overview

The system consists of a hardware fixture and and successiv software code to transform this finally to a measurement value for a database input.

<img src="./images/overview.png">


| Component | 	Usage  |	Link |
|:--------------:|:-------------|:--------|
| Mechanical Fixture |	Hardware components to fix a camera and illumination on a water meter  | [https://www.thingiverse.com/thing:3238162](https://www.thingiverse.com/thing:3238162)  |
| Taking pictures |	ESP8266 based html server to provide pictures from the camera  | [https://github.com/jomjol/water-meter-picture-provider](https://github.com/jomjol/water-meter-picture-provider)  |
| Alignment and decomposition |	Image processing with OpenCV library to extract the needed features  | n.a. |
| OCR for full digits |	Usage for OCR to extract the m³ part of the water meter  | [https://github.com/jomjol/neural-network-digital-counter-readout](https://github.com/jomjol/neural-network-digital-counter-readout) |
| Analog to Digital Readout |	Usage of a Neural Network to digitalize analog pointers | [https://github.com/jomjol/neural-network-analog-needle-readout](https://github.com/jomjol/neural-network-analog-needle-readout) |
| To Database |	Process digitalized numbers and insert into a database | n.a. |