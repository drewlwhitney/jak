# Just Another Keyboard
It's Just Another Keyboard that amalgamates the [Corne](github.com/foostan/crkbd), [Ferris Sweep](https://github.com/davidphilipbarr/Sweep), and [Fifi](https://github.com/raychengy/fifi_split_keeb).

![wireless_physical](./images/wireless-physical.jpg)
<sub>Fully assembled wireless version with [keycaps from Nuphy](https://nuphy.com/collections/keycaps/products/coast-dawn-nsa)</sub>


![wired_physical](./images/wired-physical.jpg)
<sub>Fully assembled wired version, using the same keycaps as above</sub>

## Notable Features
- Designed for [Gateron KS-33 Low Profile Switches](https://www.gateron.co/products/gateron-low-profile-mechanical-switch-set) with hotswap sockets

- Uses the Seeed Studio XIAO microcontroller with either the [`RP2040`](https://www.seeedstudio.com/XIAO-RP2040-v1-0-p-5026.html) variant (for wired builds) or the [`XIAO-BLE`](https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html) variant (for wireless builds)

- 2-pin JST connector for the battery in wireless builds

- USB-C full duplex USART communication for wired builds. None of that [TRRS nonesense](https://gabevenberg.com/posts/stop-using-trrs/)!

- [Switch plates](./switch-plate/) you can order with the PCB

- [3D printable cases](./case/) that exactly fit the boards with a battery or USB-C connectors

## Build Guide
Refer to the [Build Guide](./docs/build_guide.md).

## Firmware Guide
### ZMK
You can use ZMK with *either* the wired or wireless version of the keyboard.

- Follow the [usual setup steps for ZMK](https://zmk.dev/docs/user-setup).

- Add the `zmk-keyboards-jak` module by following the instructions on the [module's GitHub](https://github.com/drewlwhitney/zmk-keyboards-jak).

- For wired builds, follow the extra steps on the [module's GitHub](https://github.com/drewlwhitney/zmk-keyboards-jak).

- Build and flash the firmware.

### QMK
You can use QMK with the **wired version only**.

- Follow the [usual setup steps for QMK](https://docs.qmk.fm/newbs).

- Clone the [keyboard description repo](https://github.com/drewlwhitney/qmk-keyboards-jak) into your `qmk_firmware/keyboards` folder and rename it to `"jak"`.[^1]

- Follow the build instructions from the [keyboard description repo](https://github.com/drewlwhitney/qmk-keyboards-jak).

[^1]: If there is a better way to do this, please open an issue to let me know!
