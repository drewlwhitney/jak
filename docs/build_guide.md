# Build Guide
Building a keyboard like this consists of purchasing components, soldering the components, installing switches and keycaps, and possibly assembling the case. For walk-throughs, refer to the [wireless Corne guide](https://docs.typeractive.xyz/build-guides/corne-wireless) (which is not a one-to-one guide for this keyboard, but has some useful tutorials).

## Bill of Materials
The provided links are components I know work, but feel free to use any other sellers/compatible components.

### General
- 1x [PCB Set](../pcb/)

- 2x Pro Micro-Compatible Controllers<sup>1</sup> (such as [this one](https://keeb.io/products/rp2040-pro-micro-usb-c-controller))
    - I recommend socketing the controllers so you can easily remove them if needed. I like [these](https://typeractive.xyz/products/ez-machine-sockets-and-headers) sockets and headers

- x36 [1N4148W Diodes](https://typeractive.xyz/products/smd-diodes)

- x36 [Gateron Low Profile Hotswap Sockets](https://www.gateron.co/products/gateron-low-profile-mechanical-switch-set)

- x36 [Gateron KS-33 Low Profile Switches](https://www.gateron.co/products/gateron-low-profile-mechanical-switch-set)

- x36 Low Profile Keycaps (such as [these](https://nuphy.com/collections/keycaps/products/coast-dawn-nsa?_pos=16&_fid=607ff251a&_ss=c))

- 2x [GSPTS003903 Reset Buttons](https://www.digikey.com/en/products/detail/c-k/GSPTS003903/10071715)

- 2x [Switch Plates](../switch-plate/)

- (optional) 1x [3D Printable Case](../case/) (left and right)
    - If using the case, you'll also want 8x 6mm M2 screws

<br>
<sup>1</sup> For wireless builds, use nice!nanos instead

### Wireless-Specific
Buy these components in addition to those in the [`General`](#general) section for wireless builds:

- 2x [nice!nanos](https://typeractive.xyz/products/nice-nano) (*which serve as the Pro Micro Controllers*)

- 2x [JST Connectors](https://typeractive.xyz/products/battery-jack) for batteries

- 2x Lithium Batteries
    - The [301230 110mAh Battery](https://typeractive.xyz/products/lithium-battery-110mah) with a JST connector fits well under the nice!nano with the above sockets and headers.
    - Otherwise, you can use a larger battery on the underside of the PCB, such as [this one](https://typeractive.xyz/products/lithium-battery-750mah).
- 2x [Power Switches](https://typeractive.xyz/products/power-switch)


### Wired-Specific
Buy these components in addition to those in the [`General`](#general) section for wired builds:

- 2x [PCB-Flush USB-C Connectors](https://www.digikey.com/en/products/detail/gct/USB4505-03-0-A/15283201) to connect the two halves

## Notes
- For wireless builds:
    - If using the 301230 lithium battery with tall sockets/headers, solder the JST connectors to the top of the PCB (using the holes closest to the reset buttons).
    - If using a larger battery, solder the JST connectors to the bottom of the PCB (using the holes furthest from the reset buttons).
    - Ensure the polarity of your batteries matches the markings on the PCB. [These batteries](https://typeractive.xyz/products/lithium-battery-110mah) have the correct polarity, but there is no consistent standard for JST connectors.
- For wired builds, solder the USB-C connectors to the bottom side of the PCB.
