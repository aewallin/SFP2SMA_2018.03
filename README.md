# SFP-2-SMA Board, 2018-03

This is a simple board for opto/electric and electro/optic conversion of RF-signals (up to maybe 500 MHz)
using telecom SFP transcievers. The board can be fitted with either BNC or SMA connectors. It has one input
which modulates the TX pins of the SFP, and two identical outputs that represent the signal on the RX pins
of the SFP.

Some notes from 2018-04: http://www.anderswallin.net/2018/04/500-mhz-sfp-board-v4/

## Circuit description

Differential (100 Ohm) signals on the TX+/TX- and RX+/RX- pins of the SFP are converted to
single-ended (50 Ohm) signals using Mini-Circuits ADT2-1T transformers.
LMH6702 op-amps amplify/buffer all signals.
LT1963 and LT3015 low-noise LDOs provide +3V3, +6V, and -6V DC rails.
The +3V3 LDO needs heat-sinking, especially with long-range SFPs that have high current draw.

## Links to other SFP-boards

- https://osmocom.org/projects/misc-hardware/wiki/Sfp-experimenter
- https://osmocom.org/projects/misc-hardware/wiki/Sfp-breakout
- https://vksdr.com/pmod
