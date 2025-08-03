# EasySMX X10 AC695X Firmware Reverse Engineering

## What’s This?

This repo is for deep-dive RE (reverse engineering) of the EasySMX X10 game controller based on the JieLi AC695X chip. The main pain point: the controller shuts off after 5 minutes (power timeout). The bigger goal: break down the firmware, document internals, mod behavior, and enable custom hacks.

## Why?

- **Controller keeps timing out.** Annoying and unnecessary.
- **Firmware is a black box.** JieLi isn’t releasing docs.
- **We want control.** Whether it’s disabling timeout, customizing functions, or porting code, this repo is the research ground.

## What’s Here?

- **Original firmware dumps.**
- **JieLi AC695X SDK (unofficial, see credits).**
- **Disassembly/IDA/Hex dumps.**
- **Scripts, notes, and anything useful for RE.**

## Credits

- Thanks to [christian-kramer](https://github.com/christian-kramer/JieLi-AC690X-Familiarization) for the SDK .

## LEGAL: FOR RESEARCH ONLY

All content is for educational, research, and interoperability purposes under fair use. No warranty, no support, no claims. If you’re JieLi or a copyright owner and have an issue, open a polite issue first.


## What’s Already Been Tried?

- **Binwalk on firmware files:** Provided no meaningful extraction. The images aren’t standard containers, so there’s nothing obvious to unpack.
- **IDA Pro and hex editing:** No real breakthrough yet. Disassembly is messy and hasn’t uncovered the flashing routine or how to load a modded firmware file. We’ll keep digging, but expect roadblocks.
