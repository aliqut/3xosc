# 3xOsc
3xOsc | 3 VCO Eurorack Module

![render](/renders/3xosc.png)

This is a Eurorack format VCO synth module, based on Moritz Klein's VCO design.

The module was designed using KiCad.

---

**Features**:

Each of the 3 oscillators has:
  - Coarse and fine tuning knobs
  - a PWM (Pulse-width Modulation) knob
  - a FM (Frequency Modulation) knob and CV (Control Voltage) input

Controls unique to each oscillator:
- Oscillator 1:
  - Saw/Pulse switch
- Oscillator 2:
  - Saw/Pulse wave mix knob
- Oscillator 3:
  - Saw/Pulse switch
  - PWM modulation input, and modulation amount knob 

# Build Guide
- Download the Gerber files from each board's '.gerbers' folder
- If you want to make any modifications to the schematics, download the schematics, make your modifications, and create new Gerbers
- Create the BOM file containing the bill of materials
- Order all the components needed
- Send the Gerber files for PCB manufacturing, you can use [PCBShopper](https://pcbshopper.com/) to compare prices across various manufacturers.

In addition to the components in the schematic, you will need M3 bolts to mount the module into your case, and hex nuts to mount the front panel onto the components (these should come packaged with all the interface components).

Once you have your PCBs and components, refer to the BOM and schematic to solder the components onto the board.

The module is split into three boards, the main board, the connector board, and the front panel. You can make your own front panel if you'd prefer, the front panel board has no electrical connections and is purely aesthetic.
The main and connector board are connected via the pin headers on the top and bottom of the PCBs, make sure you orient the pin headers properly before soldering. The front panel is secured onto the connector board using hex nuts.

### Front Panel
_To view the front panel on KiCad, you need to install the fonts in the `fonts/` folder from this repo, or replace them with your font of choice._

To get the shiny gold finish for the exposed copper used for text/graphics, make sure you get your PCB manufactured with an ENIG finish. Most PCB manufacturers offer this as an option.

I went for a black solder mask, but you get the option to choose from many different colours when ordering your PCB.

# Contributing
Pull requests are the best way to propose changes to the schematics.

1. Fork the repo and create your branch from `master`.
2. Make your changes to the design.
3. If your change directly affects the module's functionality, update the documentation.
4. Issue pull request

## Any contributions you make will be under the MIT Software License
In short, when you submit code changes, your submissions are understood to be under the same [MIT License](http://choosealicense.com/licenses/mit/) that covers the project.

## Report issues using Github's Issues tab.
I use GitHub issues to track public bugs. Report a bug by opening a new issue.

**Issue Reports** tend to have:

- A quick summary and/or background
- Steps to reproduce
  - Be specific
- What you expected would happen
- What actually happens
- Notes (possibly including why you think this might be happening, or stuff you tried that didn't work)
