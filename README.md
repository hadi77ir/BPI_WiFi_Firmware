# Wireless Connectivity Firmware for Banana Pi Boards

This fork just adds PKGBUILDs to [upstream](https://github.com/BPI-SINOVOIP/BPI_WiFi_Firmware).

## Available Packages
|  Wireless Chipset  |           Package           |    Directory     |
|--------------------|-----------------------------|------------------|
|  AP6210            |  `firmware-ap6210-bpi`      |  `ap6210`        |
|  AP6212            |  `firmware-ap6212-bpi`      |  `ap6212`        |
|  RTL8192EE         |  `firmware-rtl8192ee-bpi`   |  `rtl8192ee`     |
|  RTL8723BU         |  `firmware-rtl8723bu-bpi`   |  `rtl8723bu`     |
|  RTL8821CU         |  `firmware-rtl8821cu-bpi`   |  `rtl8821cu`     |
|  RTL8812AE         |  `firmware-rtl8812ae-bpi`   |  `rtl8812ae`     |
|  RTL8821CU         |  `firmware-rtl8821cu-bpi`   |  `rtl8821cu`     |
|  RTL8822BE         |  `firmware-rtl8822be-bpi`   |  `rtl8822be`     |

## Which package should I use?

|          Board          |  Wireless Chipset  |           Package           |
|-------------------------|--------------------|-----------------------------|
|  Banana Pro             |   AP6210           |  `firmware-ap6210-bpi`      |
|  Banana Pi M1+          |   AP6210           |  `firmware-ap6210-bpi`      |
|  Banana Pi M2 Berry     |   AP6212           |  `firmware-ap6212-bpi`      |
|  Banana Pi M2+          |   AP6212           |  `firmware-ap6212-bpi`      |
|  Banana Pi M2U          |   AP6212           |  `firmware-ap6212-bpi`      |
|  Banana Pi M2M          |   AP6212           |  `firmware-ap6212-bpi`      |
|  Banana Pi M2 Zero      |   AP6212           |  `firmware-ap6212-bpi`      |
|  Banana Pi M3           |   AP6212           |  `firmware-ap6212-bpi`      |
|  Banana Pi M64          |   AP6212           |  `firmware-ap6212-bpi`      |
|  Banana Pi P2 Zero      |   AP6212           |  `firmware-ap6212-bpi`      |
|  Banana Pi S64 Core     |   AP6212           |  `firmware-ap6212-bpi`      |
|  Banana Pi M4           |   RTL8821CU        |  `firmware-rtl8821cu-bpi`   |
|  Banana Pi / AiWorld P1 |   AP6181           |  Not available in upstream  |


Note: "M2" boards (M2 Berry, M2+, M2U, M2M, M2Z) may be available with other chipsets (AP6181 and AP6335) too. Check your board before installing pacakges and reporting issues to this repository or upstream.

## Installation
### Prebuilt Packages
Prebuilt packages are available at [here](https://github.com/hadi77ir/BananaPi-Wireless-Firmware/releases/latest).

Prebuilt packages can be installed through:
```
# pacman -U <FILENAME>
```
where `<FILENAME>` would be the name of package file.

### Building
Clone this repository by executing
```
$ git clone https://github.com/hadi77ir/BananaPi-Wireless-Firmware.git
```
Then go to the respective directory (for example `ap6212`)
```
$ cd BananaPi-Wireless-Firmware
$ cd ap6212
```
Now you can build the package by running
```
$ makepkg -s
```
If you want to build and install using single line of command, run this instead
```
$ makepkg -si
```

## Issues and Pull Requests
Pull requests about PKGBUILDs are welcome. I don't accept any pull requests about firmware changes. Issues about the firmwares should be reported to upstream, as I am only responsible for packaging.

## License
PKGBUILDs are licensed under MIT. Check `LICENSE.PKGBUILD`. I have no rights on firmware.
