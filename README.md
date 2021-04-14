# [ Description ]
The Sand Ortholinear is a QWERTY style keyboard with 47 individually programmable keys. The
keyboard is powered by an ATMEGA32U4 microcontroller running the QMK open source keyboard
firmware. The goal of this project was to design a keyboard which is compact and durable while
having a simple case.

# [ Design Requirements ]
[X] Compact/Portable
[X] Cherry MX Compatible 
[X] Ortholinear QWERTY (Grid) Layout with 2U spacebar
[X] No visible components on top side of board
[X] minimize trace presence on visible portions of top PCB
[X] Sandwich style case PCB|ACRYLIC|PCB held together with M3 Screws
[X] USB-C Connector
[X] Sturdy Construction

# [ Version History ]
## QMKDEVBRD
Prior to getting larger and more costly prototypes made I opted to 
design a smaller keypad which uses a simplified circuit compared
to the one I intend to put in the final keyboard. In addition to the basic
microcontroller circuit with ISP and USB connectivity I also opted to 
include a prototyping area with breakouts for unused uC pins. Doing so 
makes this project not only a prototype for my final keyboard design, but also
a developemnt tool to contribute to the QMK Firmware project in the future.
The QMK Development Board functions as expected and works flawlessly with 
the QMK firmware. 

## Sand v1.0
With my initial circuit verified to be in working order, I set out to design
the full size ortholinear keyboard. In refining the design I replaced the 
micro USB present in my initial design with the more modern, and reversible,
USB-C Connector. In doing so I failed to realize the need for both D- and D+ 
lines to be shorted to its respective pairing in addition to resistors  
used by the host device to determine orientation of the connector; a more 
complicated connector than I had first imagined. Additionally I added a PTC 
fuse and a schottkey diode to prevent damage caused by potential excessive 
current draw or reverse voltage scenario. Disatisfied with how large the 
diodes were on the prototype, I chose smaller diodes, too small in fact. 
Building these by hand proved problematic with the diodes as they would 
create weird feedback in the keyboard matrix if even one was soldered
incorrectly. I made the same mistake with the crystal oscillator and had to 
tack on a through hole can to the pads as I was unable to effectively solder 
the smaller oscillator. In a future design I will avoid using such small parts 
for hand soldering.

Changing focus to the mechanical/visual design of the keyboard I opted for a simple
yet elegant PCB and Acrylic sandwich. Having discovered green edged acrylic while 
looking for potential materials I began to design a piece of acrylic to fit between
the keyboard pcb and a backplate also made of FR4 (Material PCB is made of) all held together
with M3 bolts and nuts. The resulting keyboard exceeded my expectations and is very
rigid and low-profile and provides ample protection to the PCB from dust and debris.

## Sand v1.1
As a revision to my original board I added a much larger crystal oscillator that is
easy to solder and corrected flaws in my USB circuit. I opted not to change the diodes
as this was a minor revision and I already had hundreds on hand.
