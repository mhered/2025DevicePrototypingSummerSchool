# 2025DevicePrototypingSummerSchool
Notes and exercises from 2025 Device Prototyping Summer School

## Intro to PCBs
Steve Hodges

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

## Gamepad tutorial - https://github.com/devices-lab/pro2-kicad-workshop

1. Add missing buttons to pull up resistors (needed because it is a shift register not an IC)

2) Daisy chain missing neopixels

Decoupling capacitor next to the component we want to protect, stores energy and feed when large demand

3) challenge:  connect the joystick. Check the datasheet 

4. assign missing footprints for neopixels and tactile switches

CTRL-B to unshow copper fill

cross referencing between schematic and layout is very useful

## Advice 

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

save and reuse good layouts an just copy and paste text or make a dedicated sheet

add free LEDs to spare IOs
