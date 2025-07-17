# Day 1

## Contents

[TOC]

## Intro

Steve Hodges - makes gadgets. Make computers more useful with embedded hardware

Dr Lorraine Underwood - make tech easier to be creative with for educators and children 

Rory Clark / Joe Finney / Jason Alexander

Sarah Hughes / Maura Lydon / Matt Sutton 

--

floors A ground, B 1st floor etc

no room keys, they need to badge us in and out

Breakfast In Barker House Farm

--

## Unlocking a long tail of hardware - Steve Hodges

what is it? / why its useful? / how to unlock it?

George Kindsley Zipf - linguist counted words. Long tail when we plot words by frequency, also cities by population, paper popularity, people salaries.

y = 1/(x+k)**a there's always more, heavy tail distributions

Easier to plot on log-log plot 

Also applied to rank-freq distribution of movies. In 2005 it was controlled by supply so the curve was clipped. The gap is unsatisfied demand. People would have watched them if they were available. Netflix leveraged by technology: streaming, recommender systems etc to fill this gap. Same with music, books, physical books. Same with app stores.

How do we enable these long tails? platforms. On the left mega apps. On the left research apps.

Physical devices: high cost at low volumes creates gap of unsatisfied demand

SenseCam - wearable records still every few seconds. Allows to review quickly. triggers true autobiographical recall. Stimulates and consolidates ability to remember.

Right form factor, piece of hardware and software can change a life

A different thing is to make it economically viable

prototyping then production.

Proto: focus on form factor and functionality

Production: make copies, test, revision supply chain management

In the middle many things: DFM, tooling, etc

many fail in kickstarter

sharp rise in investment in the middle: cumulative investment not linear

specially true in small runs

middle activities he calls "isotyping": suppliers & partners, pre-compliance, efficiency, certificacione, reliability, process de finition... 

That's the mission of prosquared from prototype to product

devices-lab in lancaster: help people make devices + making tools to overcome the challenges of isotyping



## Pro2 network - Rory Clark

Research Assistant for pro2 network

sw + hw + functional materials > prototypes > product > adoption

3 themes:

1. emerging materials
2. isotyping (refining + scaling)
3. infrastructure for device production (packaging, logistics, returns, etc)

Co Leads: Mike Fraser + Steve Hodges. Steeering group + Advisory Board

3M pounds over 5 years cofounded with industry

Oliver Child residency in Shenzen - there's more funding available, taking applications for residencies linked to universities, check website

Check his blog

CHI Conference - Computer Human interaction, a fraction related to devices

Open Source Hardware Summit 2025 in Edinbourgh

Industry Outreach event in winter TBA

Hardy & Ellis Inventions - product to improve BOMs

## Intro to PCBs - Steve Hodges

copper
solder resist gives the color
silkscreen
through hole vs surface mounted technology
vias to connect layers: plated holes 
chips: ICs or integrated components. Inside there is a little block of silicone. packaged. other people refer to single capacitors as chips
traces are narrower in SMD. PCBs are more dense, also there is multilayer. Can have components on both side
can have blind vias and buried layers. 
No leads components
balls buried underneath
so small not even space to print the name
pin 1 markers indicated on the chip and on the silkscreen with arrow or dot. Indications for manual assy, nowadays mounted automatically 
gold plated copper to prevent oxidation exposed
FR4 is std fiber glass substrate (fire retardant)
Al helps with heat evacuation 
flexible substrates e.g. (www.besterpcba.com)
Flexy rigid: much better, components are on rigid part and wont tear the substrate. the paste is brittle.
www.pcbelec.com
Std PCBs is 1.6mm thick. Can fit up to 24 layers. Can do thinner. 
mils is 1inch/1000 (or thou)
.1mm is the thinner a trace can be reasonably
.1mm gap between traces
trace height measured in ounces (ounces of Cu per sq foot)
Each manufacturer has their design rules
www.pcbway.com/capabilities.html
 jlcpcb.com/capabilities
www.eurocircuits.com/technical-guidelines/pcb-design-guidelines/

### PCB design process - bare boards

Schematic design
Layout design
many schools of thought about ground planes: not so easy, leave the copper in
run checks
to send design there is a standard exchange format: gerber files
represent geometries. Decades old and there are no units!
v2 X have units
typically PCBs are often panellized
Best option go to a PCB manufacturer and you'll get it in a week
If you add PCBA (component installation) the advantage is even bigger
Upload also the BOM and pick and place data
SPICE - sfw to simulate circuits, but no substitute to testing a prototype

HALT highly accelerated lifetime testing - cycle relevant effects e.g. moving flex elements, temperature cycles etc

## PCB design- Gamepad tutorial - ??

https://github.com/devices-lab/pro2-kicad-workshop

1. Add missing buttons to pull up resistors (needed because it is a shift register not an IC)

2) Daisy chain missing neopixels

Decoupling capacitor next to the component we want to protect, stores energy and feed when large demand

3) challenge:  connect the joystick. Check the datasheet 

4. assign missing footprints for neopixels and tactile switches

CTRL-B to unshow copper fill

cross referencing between schematic and layout is very useful

## Advice - John ??

Keep escape hatches

TX and RX which one is which? add polarity swap jumper pair

give yourself test pads

add version numbers!

keep it in sync with kicad sheet

do basic protection:

TVS diodes

current limiting resistors

jack sockets

debugging LEDs

save and reuse good layouts and just copy & paste text or make a dedicated sheet

add free LEDs to spare IOs