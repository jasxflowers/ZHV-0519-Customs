# ZHV-0519 Customizations
![Render of the ZHV-0519 solenoid valve without a cap.](https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/ZHV-0519_Body.png)

This repository is an ongoing set of 3d-printed customizations for the ZHV-0519 pull-type linear solenoid valve (Zonhen Electric Appliances). Currently includes files for: a 2-way, 2-position, Normally Open cap and a 3-way, 2-position, Normally Closed cap (default when purchasing online). Both files are fully parametric and meant for Autodesk Fusion 360. [Original documentation for the valve can be found here.](http://www.zonhen.com/solenoid/ZHV-0519-en.html) 

## 1: Repository Structure

* `Parametric models` contains Autodesk Fusion 360 models for each caps and are fully parametric.
* `Static models` contains STL files for each cap.
* `Body` contains files for the valve's main body (e.g. for modeling enclosures).

## 2: Caps

<center><img src="https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/Valve_PortLabels.png" alt="ZHV-5019 valve with ports labeled." width="500px"><br>
ZHV-5019 valve with ports labeled.
</center>

### 2.1: 2-way, 2-position, Normally Open

![Render of the 2-way, 2-position, Normally Open cap.](https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/2P2W_NO_Cap.png)

<img src="https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/2P_2W_NO_Illustration.png" alt="Hydraulic drawing of the 2-way, 2-position, Normally Open cap." width="200px">

This design is most similar to Zonhen's Seat A interface for the solenoid valve. 

### 2.2: 3-way, 2-position, Normally Closed

![Render of the 3-way, 2-position, Normally Closed cap.](https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/3P2W_Cap.PNG)

<img src="https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/3P_2W_NC_Illustration.png" alt="Hydraulic drawing of the 3-way, 2-position, Normally Closed cap." width="200px">

This is the default Seat B interface. The key difference is the addition of a barb for the top port, which is not usually available with Zonhen's cap.

### 2.3: Port R Barbed Cover

![Render of Barbed cover for port R.](https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/Barbed_Cover.png)

![Example of barbed cover and 3-port, 2-way, NC cap on a valve.](https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/Barbed_Cover_example.png)

If you are like me, you might be frustrated because port R does not have a barb and you don't have a tube with the right ID to fit over it snuggly. Here's a barbed cover that fits over port R, and is fully parametric. Note: you'll have to make sure the minimum wall thickness matches your 3D printer's capabilities.

Unfortunately, this means that your tube's ID needs to stretch over a 3mm OD port at minimum. The cover adds a small amount of thickness to the port (by default 0.6mm).

## 3: Valve Details

<img src="https://github.com/jasxflowers/ZHV-0519-Customs/blob/master/Images/Body_CrossSection.png" alt="Cross-section of ZHV-0519 body with spring and plunger." width="500px">



### 3.1: General Features

* **Valve type:** Pull-type linear solenoid valve
* **Total weight:** 17 g
* **Voltage:** 3-48 VDC or 24-220 VAC
* **Current:** 220 mA
* **Pressure:** 0-375 mmHg / 0-0.5 Bar
* **Fluid medium:** Air (but can work with some liquids according to me lol)
* **Life cycle:** 1,000,000 cycles (on 1 second, off 1 second)
* **Insulation class:** Class B

### 3.2: Coil Data

| Duty cycle            | 100% | 50%  | 25%  | 10%  |
| --------------------- | ---- | ---- | ---- | ---- |
| Maximum "on" time (s) | ∞    | 55   | 19   | 3    |
| Watts at 20*C         | 1.6  | 3.2  | 5.4  | 16   |
| Ampere-turns at 20*C  | 300  | 424  | 600  | 948  |

### 3.3: Maintenance

If using liquids, make sure the liquid is not corrosive and that the liquid is not kept in the body orifice of the valve for extended periods of time (e.g. days is my guess). The stopper and spring come into direct contact with the liquids, which means corrosion could affect the performance of the valve. In this case, unplug the valve, remove the cap, and clean all the parts carefully.

## 4: Peripheral hardware

These are mostly notes for myself as someone who hasn't played with these devices super often. I'll most likely be trying and comparing hardware that I want to use in conjunction with the ZHV-0519.

* Hardware that seems to be useful for the ZHV-0519 (to try for myself)
  * [Using DRV to Drive Solenoids](https://www.ti.com/lit/an/slvae59/slvae59.pdf) 
  * **DRV2510-Q1:** 3-A Automotive Haptic Driver for Solenoids with Integrated Diagnostics ([datasheet](https://www.ti.com/lit/ds/symlink/drv2510-q1.pdf)).
  * **DRV8860x:** 38-V 8-Channel Serial Interface Low-Side Driver ([datasheet](https://www.ti.com/lit/ds/symlink/drv8860.pdf)). Interested in this one for flavor interface.
  * **DRV8343-Q1** 
  * **DRV8876:** Interested in this for it's current regulation features and fault feedback. Mostly for 1-2 solenoid driving in devices.
  * **Smart Switches (SiP32429)**.

## 5: To-do

- [x] Add valve body files.
- [ ] Explain basic mechanism and how the plunger affects the ports.
- [ ] Describe some peripheral hardware suggestions for beginners.

## 6: Licensing

This documentation describes Open Hardware made for [_Perfect Melon_](https://jasbrooks.net/perfect-melon) (with the support from the [UChicago Arts](https://arts.uchicago.edu)), and is under the MIT License.
