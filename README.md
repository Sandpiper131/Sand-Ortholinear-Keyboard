# [ Description ]
The Sand Ortholinear is a QWERTY style keyboard with 47 individually programmable keys. The
keyboard is powered by an ATMEGA32U4 microcontroller running the QMK open source keyboard
firmware. The goal of this project was to design a keyboard which is compact and durable while
having a simple case.

# [ Design Requirements ]
-Compact/Portable  
-Cherry MX Compatible  
-Ortholinear QWERTY (Grid) Layout with 2U spacebar  
-No visible components on top side of board  
-minimize trace presence on visible portions of top PCB  
-Sandwich style case PCB|ACRYLIC|PCB held together with M3 Screws  
-USB-C Connector  
-Sturdy Construction  

# [ Gallery ]
## Renders:
![alt text](https://github.com/Sandpiper131/Sand-Ortholinear-Keyboard/blob/main/V1.1/FIGS/SO_SIDE_FULL_RENDER.png "sand ortho render (side)")  
![alt text](https://github.com/Sandpiper131/Sand-Ortholinear-Keyboard/blob/main/V1.1/FIGS/SO_BOT_RENDER.png "sand ortho render (bottom)")  

## Schematics:
![alt text](https://github.com/Sandpiper131/Sand-Ortholinear-Keyboard/blob/main/V1.1/FIGS/SCH_SO_V1.1.png "Sand Ortho V1.1 Schematic")

## Board Layout:
![alt text](https://github.com/Sandpiper131/Sand-Ortholinear-Keyboard/blob/main/V1.1/FIGS/PCB_FRONT_SOV1.1.png "Board Layout (Front 1)")
![alt text](https://github.com/Sandpiper131/Sand-Ortholinear-Keyboard/blob/main/V1.1/FIGS/PCB_BACK1_SO_V1.1.png "Board Layout (Front 2)")
![alt text](https://github.com/Sandpiper131/Sand-Ortholinear-Keyboard/blob/main/V1.1/FIGS/PCB_BACK_SO_V1.1.png "Board Layout (Back 0)")
![alt text](https://github.com/Sandpiper131/Sand-Ortholinear-Keyboard/blob/main/V1.1/FIGS/PCB_BACKCLOSE_SO_V1.1.png "Board Close Up (Back)")

## Pictures:
![alt text](https://github.com/Sandpiper131/Sand-Ortholinear-Keyboard/blob/main/V1.1/FIGS/SHOT2_V1.1.png "Sand Ortho Shot 2")
![alt text](https://github.com/Sandpiper131/Sand-Ortholinear-Keyboard/blob/main/V1.1/FIGS/SHOT1_V1.1.png "Sand Ortho Shot 1")

# [ Version History ]
## QMKDEVBRD
The QMK Development Board is a 3x3 Cherry MX-Compatible keypad used to
prototype a keyboard circuit prior to building a larger and more expensive keyboard. 
In addition to the basic microcontroller circuit with ISP and USB connectivity a 
prototyping area with breakouts for unused uC pins is included. Doing so 
makes this board not only a prototype for a final keyboard design, but also
a useful tool for contributing to the QMK Firmware project in the future.
The QMK Development Board functions as expected and works flawlessly with 
the QMK firmware. 

## Sand v1.0
Error in USB-C Circuit, no resistors for orientation, D+/D- not shorted 
to respective pair; USB connectivity non-functional. Added protection
circuit with Schottkey Diode and PTC fuse. Diodes are too small and
difficult to solder resulting in feedback in keyboard matrix. Crystal
Oscillator is also too small and impossible to solder by hand; Resolved
using a through hole crystal soldered onto pads. 

Changing focus to the mechanical/visual design of the keyboard is a simple
yet elegant PCB and Acrylic sandwich all held togetherwith M3 bolts and nuts.  
The resulting keyboard exceeded expectations and is very rigid, low-profile,
and provides ample protection from dust and debris.

## Sand v1.1
Added larger surface mount crystal oscillator and corrected above mentioned
flaws in the USB-C circuit. Opted not to change the diodes
as this was a minor revision and the part had already been ordered in excess.
