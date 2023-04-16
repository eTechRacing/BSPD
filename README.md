# BSPD

This repository contains the hardware design files for the Brake System Plausibility Device (BSPD) used in e-Tech Racing's electric vehicle.

## Purpose
The BSPD is a non-programmable circuit that ensures the safe operation of the vehicle during hard braking events. The BSPD must open the shutdown circuit when hard braking occurs, if more than 5kW of power is being delivered to the motors for more than 500ms.

### ⚠️Warning⚠️
Please check for changes in ruling. This BSPD is designed following [FSG Rules from 2023](https://www.formulastudent.de/fileadmin/user_upload/all/2023/rules/FS-Rules_2023_v1.1.pdf).
This version of the BSPD is normally closed when not powered. This could be a potential rules issue, so consider redesigning the relay part for this to be solved.

## Additional hardware
For the BSPD to work, two sensors and a 20-30VDC supply are needed. Here are the ones used in ETR-08:
- [Brake pressure sensor](https://www.amazon.es/gp/product/B07HLKD5L1/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1) : 0.5-4.5V, 1/8", supplied with 5VDC. Bought via Amazon, 25€
- [Hall current sensor](https://www.lem.com/en/product-list/has-100s): In order to measure power, a current sensor is used, so worst case scenario is 5kW / Vmax = 8.5A.

## Installation
- To use the BSPD, follow the installation steps below:

- Connect the brake system pressure sensor to the BSPD.

- Connect the TS current sensor to the BSPD.

- Connect the BSPD to the LVMS.

- Test the BSPD to ensure proper functionality.
