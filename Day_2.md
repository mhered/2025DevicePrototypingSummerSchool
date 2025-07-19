# Day 2

## Contents

[TOC]



## Recap

Homework videos to watch:

1.	Shenzhen: The Silicon Valley of Hardware (Full Documentary) — Wired, 2016
2.	How I Made My Own iPhone – in China — Scotty Allen, 2017
3.	Eurocircuits TV — Eurocircuits channel
4.	Inside China’s Future Factory — Ashlee Vance, Business Week, 2019
5.	You must Unlearn what You have Learned — Eric Bogatin, Altium Live 2020

Steve Hodges sensecam and micro:bit

Today Simon Munk (Sparkfun)

Tomorrow: Pete Lomas involved in the Pi

ENG2 building

## Printed circuits part 2

PCBs are panelized with a frame or rails

to separate them easily or mouse bites or rats teeth > small holes

V-scores becoming more popular > notches on both sides. must run straight all the length



form factors: solder wire, bars, solder paste for SMD

sizes: wire diameter, paste ball size

composition: lead-free or leaded > soldering tin + lead popular for prototyping easier to solder than lead-free

flux: rosin, water soluble, no-clean ? > fumes from rosin can be harmful.-. ideally halide free. ideally no-clean some fluxes are corrosive over time and must be cleaned. 

solder paste is sticky. we can heat up with solder or hot air.

we call it solder reflow

apply solder paste with a syringe. hard to get the amount right

we create a gerber layer on the areas where we want solder paste and make a metal stencil you putthe paste with a scraper

you can order stencils from the PCB manufacturer

there are also machines to apply the paste with stencils and even paste printing machines

pick and place: full manual with tweezers, semi-automatic with feeders and a pantographer for fine handling (www.fritsch-smt.de) automatic pick and place https://rushpcb.com with cameras, one or multiple heads with vacuum

need an oven to solder. Need a particular temperature profile either in place or playing with a conveyor belt

inspection AOI (automated optical inspection) sunzontech.com alpha x series

these steps are arranged in an assy line

www.tsl.com

## Scaling your prototype - Mandy Xiang

Shenzen - mandy.xiang1011@gmail.com

Device Skin (Packaging), Gut (PCB, PCBA), Skeleton (enclosure, mechanical parts, Soul (sfw, firmware)

Triangle of manufacturing: Cost, Quality, Schedule

Cost: you see manufacturing, tooling, BOM but hidden costs: defects, mistakes, certification, logistics, engineering, management, marketing, taxes...

Schedule: project management is critical supply chain is dynamic

Quality: aligning expectations

### Design from manufacturing

designer should be responsible for what you started including manufacturing

Design for X

need a bigger team: software is a band, hardware is an orchestra

highest risks: 

* injection molding (35-45 days), 
* customized parts due to lead time and tolerances

Gerber files and PCB specs 

### PCB DFM hints

top failure sources: component mismatch with pad, missing polarity marks, missing pick and place x-y data 

100 popular components cover 30% of BOM

open hardware for sustainability

### Test and Quality

 Reliability tests: thermal shock, humidity, temperature, dye and pry, cross section, pull and shear test, Certifications: FCC, CE, UL, RoHS, REACH WEEE etc

### Takeaways

verification

DFM critical especially for molding

consider hidden costs

prioritize SMD and popular components (cheaper, easier to source)

local vendors: through open parts SEED or preferred parts JLC

JLC is prominent > expanding to provide access to local services

problem: if they dont have the components you need to buy yourself and ship to them

one stop services provide PM, DFM and sourcing

## SMD practical workshop

Lessons learned:

- process
  1. put a drop of solder in one pad
  2. reflow while pushing the component with tweezers
  3. if necessary reflow and reposition
  4. solder the remaining pads
- look out for pin 1 markings (dots) in devices where polarity matters
- work in batches
- test when possible
- ventilation



## 1 min madness

Abi Choi - 3D printing computer viion

Anh Pham . 

Are-Wolf - wearables

Beccy Abraham - collaborative music

Ben Seleb - sled dogs, field sensors, wildlife

Charly Olivier - maker, programmable car French

Chris Courage - creative coding. ciclist. coding club. previously CNC machining

Chris Lowerson - army, cyber security. passion for education. 

Christian Grose - sewing MEch Eng & Design

Dalya AlShahrabi - jordan > Northumbria

Dongyi - Beijing Telco + connected environments. PhD. urbanheatsense.com

Emma Derby Hansen - Danish / Malmo. games and mechatronics, digital fabrication

Hannah van Iterson - phd industrial design embodied systems for preentive healthcare

Heather shaw - derby, psychology 

Iman Hussain - PhD indoor air quality 

Jamie Glen - graduated

Jan Kucera - Check .net gadgeterr script encoding ??

Jonathaan Sanderson - nustem learning with family computational tinkering jjsanderson

jooyound Park - Sweden dance wearables menstrual pain

Lewis birch - AI security@ mindgard interested in drones, 3d printing electronics

lukas rambold - Berlin inflatable structures

michael langton - manager of uni maker lab omnicom 

mordecai (moti) botrashvilty - Israel quantum, arduino

Natalie Mordi - industrial Design. 

Nick Taylor 

Patricia Cadavid - Colombia. Media Arts. Sound performance

Pranjal Jain - phd swansea. india. hardware for repairs

Ulrike (Rika) Kulzer - Ulm, informatics. PhD haptics in wearables. 

Sebastian Prost - Austria, postdoc in London sustainability, social justice, co creating, farming

Seher Singh - India psychology and HCI. 

Shyamli Suneesh - physics, robotics, arduino. robot for children 7-11

Simran Chopra - communication design and new media design. postdoc 

Sofia - Malmo Uni. half italian. Passion perfume making

Stig Konings - researcher Belgium. watchmaking, leathercraft, loves making PCB

Terry Fawden - ear worn device to analysi human emotion

Tobias Kunz - tobias.kunz@outlook.com peer mentoring group

Will Dove - will start PhD, is just graduating

Yang Gao - PhD in psychology in Oxford, originally from Beijing. NY, Abu Dhabi, film making. 

## Building an Electronics Manufacturing Business on a Shoestring - Simon Monk 

PhD Lancaster

### Intro

Book author "30 arduino projects for the evil genius" 

Monksmakes Ltd initially starter kit for RPi to go with the books 

later accesories RPi and micro:bit

possibly for makers and educators

only manufacture, no retail

### Cost of Entry

computer and kicad are free

basic electronics prototyping kit 200€: start with thru hole and perforated boards

good soldering iron 100€

SMD better to do with an oven or hot air gun

start simple

multimeter

power supply 

cheap test equipment from china 

more exotic equipment: borrow it if needed

handheld oscilloscope 100€ > aliexpress 

even spectrometers for EMI testing

order bare PCBs from JLC or PCBway and stencil al the same time

hot air gun 20-30€

toaster oven + low temp solder paste (~140C) 

reflow oven 3-400€

### Process

paper design

breadboard

order 5 prototype PCBs + stencil

BOM is maybe 10-15€, accumulate several prototypes to save on delivery

test and iterate

make automated tester if you're going to make 100s

make panelized design 20-30cm to fit 9-25 boards

make docs: datasheer, user instructions, pick and place sheet, manufacturing guide

first batch 50-200 units

### Pros and Cons DIY vs PCBA

DIY: own components, manufacture on demand small batches. Local country of origin.

PCBA: high Q, expensive for prototypes, commit to bigger batch, risky if need to evolve

### Design for Manufacturability

0603 cost .15 cents each

use stad components 150KOhm or 100KOhm

1 side 2 layers

routing is fun 

minimize TH components more expensive!

consider cost of BOM at design. a Texas Instruments voltage regulator x10 the cost. buy components LCSC.com  (JLC buy from them)  

### Scaling up

design the full panel, not the single PCB

stencil machine 200€

PnP machine 2500-7000€ (could be 70000!)

Reflow oven 200-20000 from drawer to conveyor belt

or outsource

### Sustainability

solar panels and battery

rework failures

small well stuffed card boxes

e-waste: WEEEwaste electrical & electronic equipment? need to pay

batteries: must be removable BPRN

reuse boxes

shipping: offer carbon offsetting 

### Tariffs

import cost paid by customer, only in US

depend of country of origin and harmonized tariff code (electronics usually fall under base case)

Need to do substantial transformation, repackaging or dilution with water does not count

### Compliance

CE is self-certified, policed by exception, don't have to pay

company in yorkshire have great documentation

if there's nothing high freq its unlikely to have issues. mitigate with spectrometer + near field probes to check for accidental antennas. Need to be below # of dB in a certain spectrum. Pimoroni do somethgin similar. Switching high fewm amy be an issue

RoHS restriction of hazardous substances e.g. Lead, Cadmium, Phthalates. Lab testing is surprisingly cheap. Request RoHS certificates from suppliers or send for testing. Download and keep paperwork!

EMI requirement > no interference with other devices. commercial compliance is 1000 per product

e.g. wifi and bluetooth buy a precertified modules e.g. ESP32

### Summary

Start simple

never been easier

DIY requires deep understanding. Good forums for machines

Moved from PCBWay to JLC due to a shipping mistake

JLC positions as more professional

PCBWay for hobbyists but offers transparent substrate, full color silkscreens etc

books and electronics kits are very complementary

retail is a pain. People return things and ask questions!

## CAD tutorial

pre made enclosures

3D printed laser cut

on demand manufacturing sheet metal bending, injection moulding etc



github.com/devices-lab/pro2-cad-workshop

onshape:

* cloud native

* parametric can goback in history and update everything
* free (ish) but designs are public 

Other options: Fusion 360 (only Windows and Mac), FreeCAD, OpenScad

### Onshape concepts

Part Studios: cn define sketches, features and look at the History

Sketches: lines, fillets, dimensions, dimensions, constraints

Features: Sketchs, Planes, Extrusion

Parts

Design Timeline

Assemblies: more about placing and mating parts. Can add motion mating (e.g. rotate relative to each other)

If you over constrain a sketch it goes red. Many constrains are added automatically. Undo and notice when it sis snapping and say no

STEP files

geometric exchange format

can be exported from KiCAD

3D print the step of the PCBA as rapid prototype. Similarly with batteries etc.

Use the STEP files as context, no need to measure every dimension

Onshape has very good documentation



Check https://www.shapr3d.com/pricing

Link to file: https://cad.onshape.com/documents/855a1103921c8fff01a9cc68/w/523188e6c79748246add5e02/e/e30ef65a0a969b823a4525ce
