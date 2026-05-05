# NexVLF
This is software defined radio hardware and software for VLF 40kHz to
300kHz range with high noise immunity, dynamic range, sensitivity, and
a built in 1m diameter loop antenna. It could be used to fool around
with VLF, to add a WWVB decoder to your shack (one is planned in
software), or whatever you like.

# Architecture

NexVLF uses an STM32H753 microcontroller to control and shovel bits
from the AK5572 24-bit audio codec into a USB2 (480Mb/s "high speed")
audio interface. A host CPU runs an app built for Linux, MacOS, and
Windows supplying the DSP functions to demodulate and tune the SDR
samples and a flexible and easily extensible receiver GUI mostly
written in Lua.
