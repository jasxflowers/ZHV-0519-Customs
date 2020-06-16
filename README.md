# ZHV-0519 Customizations
This repository is an ongoing set of 3d-printed customizations for the ZHV-0519 solenoid valve (Zonhen Electric Appliances). Currently includes files for: a 2-port 2-way Normally Open cap and a 3-port 2-way Normally Closed cap (default when purchasing online). Both files are fully parametric and meant for Autodesk Fusion 360. [Original documentation for the valve can be found here.](http://www.zonhen.com/solenoid/ZHV-0519-en.html) 

## Repository Structure

* `Parametric models` contains Autodesk Fusion 360 models for each caps and are fully parametric.
* `Static models` contains STL files for each cap.

## Maintenance

If using liquids, make sure the liquid is not corrosive and that the liquid is not kept in the body orifice of the valve for extended periods of time (e.g. days is my guess). The stopper and spring come into direct contact with the liquids, which means corrosion could affect the performance of the valve. In this case, unplug the valve, remove the cap, and clean all the parts carefully.

## Caps

### 2-port, 2-way, Normally Open

![Render of the 3-port, 2-way, Normally Open cap.](https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/2P2W_NO_Cap.png)

<img src="https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/2P_2W_NO_Illustration.png" alt="Hydraulic drawing of the 2-port, 2-way, Normally Open cap." width="200px">

This design is most similar to Zonhen's Seat A interface for the solenoid valve. 

### 3-port, 2-way, Normally Closed

![Render of the 3-port, 2-way, Normally Closed cap.](https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/3P2W_Cap.PNG)

<img src="https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/3P_2W_NC_Illustration.png" alt="Hydraulic drawing of the 3-port, 2-way, Normally Closed cap." width="200px">

This is the default Seat B interface. The key difference is the addition of a barb for the top port, which is not usually available with Zonhen's cap.

## Valve Details

To make the information for the valves more readily accessible - as Zonhen only provides it as an image - I've copied it over as tables below.

### General Features

* **Total weight:** 17g
* **Voltage:** 3-48 VDC or 24-220 VAC
* **Pressure:** 0-375 mmHg / 0-0.5 Bar
* **Fluid medium:** Air (but can work with some liquids according to me lol)
* **Life cycle:** 1,000,000 cycles (on 1 second, off 1 second)
* **Insulation class:** Class B

### Coil Data

| Duty cycle            | 100% | 50%  | 25%  | 10%  |
| --------------------- | ---- | ---- | ---- | ---- |
| Maximum "on" time (s) | ∞    | 55   | 19   | 3    |
| Watts at 20*C         | 1.6  | 3.2  | 5.4  | 16   |
| Ampere-turns at 20*C  | 300  | 424  | 600  | 948  |



## Licensing

This documentation describes Open Hardware made for [_Perfect Melon_](https://jasbrooks.net/perfect-melon) with the support from the [UChicago Arts](https://arts.uchicago.edu) and is under the MIT License.
