---
layout: project
type: project
image: images/micromouse.jpg
title: PID Control of a Servo Motor with Raspberry Pi
permalink: projects/hardware
# All dates must be YYYY-MM-DD format!
date: 2020-12-01
summary: loren ipsum dolores 
---

---
---

# Outline:
- [Project Management](#project-management)
- - [Time](#project-management-time)
- - [Cost](#project-management-cost)
- - [Scope](#project-management-scope)
- - [Resources](#project-management-resources)
- - [Risk](#project-management-risk)
- - [Quality](#project-management-quality)
- [Design Process](#design-process)
- [Bill of Materials](#bill-of-materials)
- [Component Analysis](#component-analysis)
- - [l298N Breakout](#component-analysis-l298n)
- - [Rotary Encoder](#component-analysis-encoder)
- - [Nema 17 Stepper Motor](#component-analysis-nema)
- - [Rapsberry Pi 4](#component-analysis-raspberrypi)

---
---

## Project Management {#project-management}
2020-12-30

- Time  (T) = 
- Cost  (C) = 
- Scope (S) =


- Resources (R) =
- Risk      (P) =
- Quality   (Q) = 


### Time {#project-management-time}

### Cost {#project-management-cost}

### Scope {#project-management-scope}
- Project Schematic
- Bill of Materials
- Documentation of Components
- Set of demonstration tests

### Resources {#project-management-resources}

> 1. Kicad 

### Risk {#project-management-risk}

### Quality {#project-management-quality}

---
---




## Bill of Materials {#bill-of-materials}

| Component | Price |
| :-------: | :---: | 
| [Rotary Encoder](https://www.amazon.ca/gp/product/B07JM9YRTQ/ref=ppx_yo_dt_b_asin_title_o05_s00?ie=UTF8&psc=1) | 28.99 | 
| [Batteries](https://www.amazon.ca/gp/product/B00MNV8E0C/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1) | 17.77 |
| [Battery Holders](https://www.amazon.ca/gp/product/B07BNMKNQX/ref=ppx_yo_dt_b_asin_title_o00_s01?ie=UTF8&psc=1) | 12.99 |
| [Hook Up Wire](https://www.amazon.ca/gp/product/B01EV70C78/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1) | 13.99 |
| [Worm Gear Motor](https://www.amazon.ca/gp/product/B073S5GM6Q/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1) | 27.79 |
| [L298N Motor Driver](https://www.amazon.ca/gp/product/B00CAG6GX2/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1) | 13.98 |
| [Raspberry Pi Model 4](https://www.amazon.ca/gp/product/B07YCWRZ8P/ref=ppx_yo_dt_b_asin_title_o01_s01?ie=UTF8&psc=1) | 149.99 |
| [Raspberry Pi GPIo Breakout Cable](https://www.amazon.ca/gp/product/B07425G6D6/ref=ppx_yo_dt_b_asin_title_o05_s00?ie=UTF8&psc=1) | 11.99 |
| **Total** | 277.00 |

---
---
## Design Process {#design-process}

### Schematic

### PID

### Demonstration

#### Limitations

---
---
## Component Analysis {#component-analysis}

### L298N Breakout {#component-analysis-l298n}

<img src="https://images-na.ssl-images-amazon.com/images/I/71Zb8MKCTtL._SL1500_.jpg" width="200" height="200" />

[Datasheet](https://www.st.com/resource/en/datasheet/l298.pdf)

### Rotary Encoder {#component-analysis-encoder}

<img src="https://images-na.ssl-images-amazon.com/images/I/61C0Cj7TiUL._AC_SL1001_.jpg" width="200" height="200" />


Information
- Output :AB 2phase output rectangular orthogonal pulse circuit, the output for the NPN open collector output type (needs pull-ups)
- AB 2phase output must not be directly connected with VCC, otherwise, will burn the output triode, because different batches, and may not have the terminal.(Green = A phase, white = B phase, red = Vcc power +, black = V0)​
- Voltage - DC 5-24 V

### Nema 17 Stepper Motor {#component-analysis-nema}

<img src="https://robu.in/wp-content/uploads/2017/12/ROBU-5.jpg" width="200" height="200" />

<img src="http://www.robotdigg.com/crab/image/2017/04/26/298d5b8abefcf8769a09fac124da0619.jpeg" width="800" height="400" />

Information
- Rated voltage (4.54 V)
- Rated Current (0.84 A)

### Raspberry Pi 4 {#component-analysis-raspberrypi}

<img src="https://images-na.ssl-images-amazon.com/images/I/41lgsFPaTnL._AC_.jpg" width="300" height="200" />

Logic levels 3.3V

Output
- Total max current (all pinis) 50 mA
- Default 8 mA max per pin
- Don't drive capacitive loads

Input
- Threshold of 1.8V
- Max of 0.5 mA
- Use 6 KOhm res to ensure 3.3V source cannot exceed 0.5 mA (3.3 V / 6000 Ohm = 0.00055 A)

---
---