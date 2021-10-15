
# Redwood - PCB 0.1.0

The main changes are:
- Trace fixes
- Better tenting puck screw clearance
- Optional haptic feedback, trackball and rotary encoder.
- TRRS or TRS cable
- Smoother board edge profile
- Rename to Redwood

## Known Issues

The haptic kex mount standoff might touch both the SCL and the unused D4 castellated pins on the MCU side. A 5mm diameter standoff looks to be doing that. Electrical tape along the MCU side should prevent any issue. The next PCB will move them further apart.

## Details

- Haptic header, mounts and I2C resistor SMT pads
- Trackball mount points
- TRRS jack on the side of the board
- All thumb keys wired as bottom row, so only six columns in matrix
- LEDs just above keys, so not less eye glare
- Column and row pins lower on MCU
- Bottom and top copper ground planes
- Vertical traces follow switch path and go through diode gaps
- Outer column trace is brought down earlier, so the cutout area is cleaner.
- Fixed acid traps on LEDs and some switches
- Board name label in lower center

## Footprint Changes
- Choc-diode traces redone; diode silk end bar not cut off
- Choc switch trace to pad angle has more margin  
- Choc switch SMT pad traces are symetric with vias off pad
- LED ref numbers on fabrication layer not silk
- TRRS jack works with TRS and TRRS cables
- Pimoroni Haptic footprint with 1x5 header, mount point, and rough outline
- TRRS symbol and footprint clear with T, R1, R2, and S pin labels

# LongFir - PCB 0.1.0-alpha-1

Broken: For each switch there is no trace connecting the two side vias to the diode, though there is a channel in the copper fill plane for one. The two traces in the switch footprint did not make it to the gerber, nor the 3D view.

## Features

- 48 keys
	- Choc spacing and switches
	- Aggressive column stagger of Ferris
	- Four thumb arc lower plus one upper
	- Outer pinky column breaks off
	- Extra key under ring column
- Tenting puck mount points
- TRRS point up for use over laptop
- Underglow with six SW6812-MINI-E
- 100 x 141 mm and reversible
- MCU daughter board
- Soldered switches

## Know Issues

- Traces within switch footprints not in Gerber
- Diode silk solid bar not visible

## What worked

- Switch locations work, with tweezers....
- LEDs work
- LEDs fit nicely between switch bodies. Slight room in cutout is good. Not sure if pads are long enough.
- LEDs shine through PCB edge and up when no solder mask

# LongFir - PCB 0.1.0-alpha-0

Not fabricated. Drill files were out of sync with gerber files.