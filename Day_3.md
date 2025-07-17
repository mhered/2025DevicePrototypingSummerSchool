# Day 3

## Contents

[TOC]



## Raspberry Pi - Scale-up or oblivion - Pete Lomas

cofounder of RPi foundation

pete@norcott.co.uk

1M cores neuromorphic computer

models 1/16 of mouse brain and consumes 100KW

computation to power consumption ratio will be key in the future

if you dont know you have to ask

know who to ask

6 founders. He was manuf engineer

RPi was designed in Cheshire

use really nice graphics

MVP was difficult then they shifted to ARM

interview on BBC with rory Cellan-Jones a 15pound computer

started thinking they'd do 3000 you can do compromises. Subsidize. If you scale costs do matter.

Target: should cost same as a text book so you should risk breaking it

Target: 

$25 model A 

35$ model B

dont let marketing get ahead of engineering

minimum viable product. it builds or destroys a brand

test market and prove manufacturability

the minimum and many "wants" be ruthless otherwise you en up with a bloated product

be analytical about it: is it critical to the mission? what is the cost to implement? can it be part of a premium product or an addon?

In their wildest dreams they based their cost model in 20k they got 200k expressions of interest!

200k is 5M$ worth of stock! How to finance? Not possible to do it progressively too slow

decide to license Farnell and RS the make, distribute, sell

UK registered charity had some rules

On launch day overwhelmed they sold everything in minutes. Farnell, RS, and their website

product assasin bug - if you see something not right follow it or it will come back and bite you

hardware bugs not easy to fix!

subtle defects

35$ product, replacement costs 190$ > quality is critical!!

with volume prices drop

2012 raspberry comes to wales with sony

Raspberry Pi 5 almost all features are in! 4M units sold!

RPi 1 was done pro bono, Pi5 costed millions. Is it right for a charity?

success due to building a community, the GPIO

ability to connect a fully fledged computer: light an LED programmed with scratch



## From Prototype to Product with LOOP - Kim Sauve

perception for physical data

applied design

loop displays activity tracker data

laser cutting, complex assembly, durability, repair cost etc

## Scaling from Prototype to Product - Steve Hodges



prototyping easier than ever, lots of tutorials, maker spaces, tech shops

isotyping is hidden and hardware is hard

papers on low scale manufacturing

75% creators 25% enablers (manufactorers helping or investors)

patterns and mitigation strategis

gaps in technical knowledge:

* no clear path to learn, relaying on word-of-mouth
* learning from mistakes

gaps in non-tech knowledge:

* finance, marketign, distribution, customer service
* you need more budget
* pricing product too low
* 50% never made a profit even after many years

lack of rigor in preparation:

* even you know you have to do it but don't have the discipline
* e.g. sloppy documentation, not following sourcing of parts etc

building relationships and a professional network

* network of partners for recommendations and intrductions
* strong relationship with manufacturing partner. Visit in person

### Minimum viable rigor

clean schematics: comments, label nets, component information, versioned

Use drawing block: info, version numbers!! You will need to iterate

Use a variable to keep it in drawings, silkscreen and name of gerbers

Come up with a robust process when you make changes: Engineering Change Order

standard operating procedure well documented one source of truth

### DFM

understand how it will be produced and match these processes

encompasses manufacturing, assembly, quality, cost, compliance and sustainability

Design "from" manufacturing by SEEED studios:

- use parts from other products and retrofit it. Leverage existing investments to reduce cost and risk

e.g. reused MP3 player enclosure for an oscilloscope

### Indoor Air Quality Trilemma - Iman Hussain

90% of time indoor. Air pollution linked to academic performance. Children particularly vulnerable. 

affordable intuitive sensor to help decisions 

## Prototyping for Research - Bringing Sciene to Industry - UrbanHeatSense.IoT - Dongyi Ma

LoraWAN network in London 68 sensors hyperlocal temperature differences

low cost heat sensors

wireless

v1 arduino with battery

v2 solar powered

v3 citizen science version. custom PCB > 30GBP

## StoryStick++ Rethinking Measurement in the Maker Age- Stig Konings

measurements are difficult and error prone, best practices unwritten

HCI > shift burden of usability to the tool itselft

original story stick is a block with notches for a given task

## Floral Scent Clock - Yang Goo

...

## Scaling up - Testing + Tooling - Steve Hodges

some times more time designing the testing infrastructure: test jig, software etc

Tooling anything to help manufacturing: mould, test jigs, paste stencils 

need repeatable process easy to do by anyone

you may need certificacion by an authorised body. They will also test e.g. for safety, EMI etc

Don't want to test the first production units

May need pre-compliance testing to avoid surprises in certification

 at some point you need to start caring about reliability and efficiency

make sure copies are faithful but also give to others to test for usability and functionality in the wild (without you there)

3 phases

1. engineering validation testing (EVT)

2. design verification testing (DVT)

3. production validation testing (PVT)

1 + 2 have we designed the product correctly?

2 + 3 have we manufactured the product correctly?

### EMC testing

electromagnetic compatibility > needed to stamp it CE and export it

law says if a product is in the market (not necessarily sold) must be EMC compliant e.g. wont interfere with a pacemaker

often manufacturers risk it without full paperwork

semi anecoic chamber: RF anecoic spikes and a wooden table (invisible to RF). Measure with antenna at 360 degrees at several heights. Need to use a suitable calibrated facility to measure  emissions. Also check if your device is overly susceptible to RF emissions. Radio and conductive emissions.

CE marking is self certified! But you need to be able to back it up if needed. Need a technical file

TEM cell TBTC1

https://www.tekbox.com/product/open-tem-cells-emc-compliance-testing/

### Production testing

Besides optical inspection, it is actually cheaper to test every unit than making the line more elaborated

sometimes harder to design the test station than the PCB

1M Xbox controllers / week > 97-98% first pass but many in the 2-3% are ok, is the test thats too aggressive. A better test would take longer. The ones at risk you run more thorough tests

### Prototype testing

order bare boards and populate it partially or partially depopulate the PCBA

CI helps. Not perfect because only checks what you have imagined but guarantees no regression

could we do something like this for hardware?

sfw not there yet to do it with simulation SPICE

LT SPICE and TINA SPICE good for analog electronic design

Frist proto is for the engineers not for the final user. Start for a bigger version

traco power dc-dc converters



## Test and measurement tools - Steve Hodges

We can only measure electrons

conventional current flow is in opposite direction to electron movement

unit of charge Coulomb

Current (A) how fast (Amp = Coulomb/sec)

Voltage (V) how much energy each coulomb has 1 V = 1J/C

Power (W) how quickly energy is delivered 1W=1J/s

### Multimeter

Voltage: need 2 probes, in parallel, not intrusive

Current: must break circuit, is intrusive 

Resistance, Capacitance...

### Oscilloscope 

measures only V but versus t very fast

cheap ones without screen connect to computer over USB

at least two channels

scope probes: beware of observer effect

fancy probes may be 1000GBP

components may have +-10% tolerance

### bench power supply

PSU

### logic analyzer

oscilloscope but measures many digital signals

outdated

### protocol analizers

read digital signals and tell you what is  communicater

now cheap logic analyzers

### PC bite sensepeek.com 

pogo pins

### jtag

40 years ago

SWD only for ARM

in circuit programming

## Volunteering to test MakeDevice

## Demo of immersive space
