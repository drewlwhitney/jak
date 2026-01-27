# Build Guide
Building a keyboard like this consists of purchasing components, soldering the components, installing switches and keycaps, and possibly assembling the case. For walk-throughs, refer to the [wireless Corne guide](https://docs.typeractive.xyz/build-guides/corne-wireless) (which is not a one-to-one guide for this keyboard, but has some useful tutorials).

## Bill of Materials
The provided links are components I know work, but feel free to use any other sellers/compatible components.

### General
- 1x [PCB Set](../pcb/)

- 2x [Seeed Studio XIAO RP2040 Controllers](https://www.seeedstudio.com/XIAO-RP2040-v1-0-p-5026.html)<sup>1</sup>

- x36 [1N4148W Diodes](https://typeractive.xyz/products/smd-diodes)

- x36 [Gateron Low Profile Hotswap Sockets](https://www.gateron.co/products/gateron-low-profile-mechanical-switch-set)

- x36 [Gateron KS-33 Low Profile Switches](https://www.gateron.co/products/gateron-low-profile-mechanical-switch-set)

- x36 Low Profile Keycaps (such as [these](https://nuphy.com/collections/keycaps/products/coast-dawn-nsa?_pos=16&_fid=607ff251a&_ss=c))

- 2x [PTS526SM15SMTR2 LFS Reset Buttons](https://www.digikey.com/en/products/detail/c-k/PTS526SM15SMTR2-LFS/10056625)

- [Switch Plates](../switch-plate/)

- (optional) 1x [3D Printable Case](../case/) (left and right)
    - If using the case, you'll also want 8x [TODO]mm M2 screws

<br>

<sup>1</sup> For wireless builds, use the `XIAO BLE` instead

### Wireless-Specific
Buy these components in addition to those in the [`General`](#general) section for wireless builds:

- 2x [XIAO BLE Controllers](https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html) (*which replace the XIAO RP2040 Controllers*)

- 2x [JST Connectors](https://typeractive.xyz/products/battery-jack) for batteries

- 2x Lithium Batteries
    - The [301230 110mAh Battery](https://typeractive.xyz/products/lithium-battery-110mah) is good for lighter boards if you don't need the battery life to last longer than a week.
    - Otherwise, you can use a larger battery, such as [this one](https://typeractive.xyz/products/lithium-battery-750mah).
- 2x [Power Switches](https://typeractive.xyz/products/power-switch)


### Wired-Specific
Buy these components in addition to those in the [`General`](#general) section for wired builds:

- 2x [Mid-Mount USB-C Connectors](https://www.digikey.com/en/products/detail/gct/USB4505-03-0-A/15283201) to connect the two halves

## Notes
- For wireless builds:
    - Ensure the polarity of your batteries matches the markings on the PCB. [These batteries](https://typeractive.xyz/products/lithium-battery-110mah) have the correct polarity, but there is no consistent standard for JST connectors.
- For wired builds, solder the USB-C connectors to the bottom side of the PCB.
- When soldering the PCB, all diodes should have the cathode on the top pad.
