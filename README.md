# About

[![OSHPark PCB Top Thumbnail](artwork/thumb_top.png?raw=true)](artwork/top.png?raw=true)
[![OSHPark PCB Bottom Thumbnail](artwork/thumb_bottom.png?raw=true)](artwork/bottom.png?raw=true)

Custom Raspberry Pi Add-on board used for launching the [Galactic Aztec] rocket. The board was designed to be stackable with other add-on boards via the designated [pin configuration].

The Camera Control ethernet port was designed to activate [HackHD] cameras via the [Galactic Aztec Camera Control] \(rev2 or newer) board and can be configured to activate multiple [HackHD]s using the [Galactic Aztec Camera Control Splitter] board.

The Valve Feedback ethernet port was designed to read valve actuation status (open or close) by means of reading Reed switches (for the Main, LOX and Kerosene valves) via the [Galactic Aztec Reed Switch Interface] and [Galactic Aztec Reed Switch Splitter] boards.

Custom EagleCAD parts on this board can be found in the [SDSU Rocket Eagle Libraries].

## Wiring
The Camera Control and Valve Feedback ethernet ports adhered to the following [T-568B] wiring configurations:

### Camera Control
| Pin | Color        | Function |
|:---:|:------------:|:--------:|
| 1   | Orange/White | In       |
| 2   | Orange       | Out      |
| 3   | Green/White  | In       |
| 4   | Blue         | Out      |
| 5   | Blue/White   | In       |
| 6   | Green        | Out      |
| 7   | Brown/White  | In       |
| 8   | Brown        | Out      |

*In and Out do not have a polarity but rather are labeled to distinguish the two sides of the camera connection (used to [control the HackHD] by means of connecting `Button Input` to `Ground`).*

### Valve Feedback
| Pin | Color        | Function |
|:---:|:------------:|:--------:|
| 1   | Orange/White | Main     |
| 2   | Orange       | Main     |
| 3   | Green/White  | LOX      |
| 4   | Blue         | 3.3V     |
| 5   | Blue/White   | 3.3V     |
| 6   | Green        | LOX      |
| 7   | Brown/White  | Kerosene |
| 8   | Brown        | Kerosene |

# Bill of Materials
| Qty | Description                             | Part Number          | Vendor   |
|:---:|-----------------------------------------|---------------------:|----------|
| 1   | Header Stacking 2x20 Tall 23mm          | [1979]               | Adafruit |
| 2   | Jack RJ45 CAT5/CAT5e                    | [380-1046-ND]        | DigiKey  |
| 2   | Header JST PH 2mm 2-pos Right Angle PTH | [455-1719-ND]        | DigiKey  |
| 1   | LED Red Vf=1.8V If=2mA 0603             | [475-1195-2-ND]      | DigiKey  |
| 1   | Molex Mini Fit Jr. 4-pos Right Angle    | [WM1352-ND]          | DigiKey  |
| 1   | LED Red Vf=2V If=20mA 0603              | [754-1359-1-ND]      | DigiKey  |
| 3   | Transistor NPN 40V 600mA SOT-23-3       | [MMBT2222ATPMSCT-ND] | DigiKey  |
| 1   | Resistor 1.8kΩ 1/4W 1% 0603             | [P1.8KBYCT-ND]       | DigiKey  |
| 1   | Resistor 1.2kΩ 2W 1% 2512               | [A116034CT-ND]       | DigiKey  |
| 3   | Resistor 1kΩ 1/4W 1% 0603               | [RHM1.00KADCT-ND]    | DigiKey  |
| 3   | Diode 50V 1A SOD-123                    | [SM4001PL-TPMSCT-ND] | DigiKey  |
| 3   | Relay 5V 5A SPST-NO (1 Form A)          | [Z945-ND]            | DigiKey  |


[Galactic Aztec]: http://rocket.sdsu.edu/rockets
[pin configuration]: https://docs.google.com/spreadsheets/d/1zGslKhH-ZteeA8sbbTjQlF-Neb-wJ3quIlFH6I8Cvgs/edit?usp=sharing
[HackHD]: http://hackhd.com/
[Galactic Aztec Camera Control]: https://github.com/twyatt/galactic-aztec-camera-control
[Galactic Aztec Camera Control Splitter]: https://github.com/twyatt/galactic-aztec-camera-control-splitter
[Galactic Aztec Reed Switch Interface]: https://github.com/twyatt/galactic-aztec-reed-switch-interface
[Galactic Aztec Reed Switch Splitter]: https://github.com/twyatt/galactic-aztec-reed-switch-splitter
[SDSU Rocket Eagle Libraries]: https://github.com/twyatt/SDSURocket-Eagle-Libraries
[T-568B]: https://en.wikipedia.org/wiki/TIA/EIA-568#Wiring
[control the HackHD]: http://www.hackhd.com/hiw.php
[1979]: http://www.adafruit.com/products/1979
[380-1046-ND]: http://www.digikey.com/product-detail/en/SS-7188-NF/380-1046-ND/388308
[455-1719-ND]: http://www.digikey.com/product-detail/en/S2B-PH-K-S(LF)(SN)/455-1719-ND/926626
[475-1195-2-ND]: http://www.digikey.com/product-detail/en/LS%20L29K-H1J2-1-Z/475-1195-1-ND/810356
[WM1352-ND]: http://www.digikey.com/product-search/en?x=0&y=0&lang=en&site=us&keywords=538-39-30-1040
[754-1359-1-ND]: http://www.digikey.com/product-detail/en/APG1608SURKC%2FT/754-1359-1-ND/1919171
[MMBT2222ATPMSCT-ND]: http://www.digikey.com/product-detail/en/MMBT2222A-TP/MMBT2222ATPMSCT-ND/717394
[P1.8KBYCT-ND]: http://www.digikey.com/product-detail/en/ERJ-PA3F1801V/P1.8KBYCT-ND/5036145
[A116034CT-ND]: http://www.digikey.com/product-detail/en/5-2176070-1/A116034CT-ND/4280086
[RHM1.00KADCT-ND]: http://www.digikey.com/product-detail/en/ESR03EZPF1001/RHM1.00KADCT-ND/1983752
[SM4001PL-TPMSCT-ND]: http://www.digikey.com/product-detail/en/SM4001PL-TP/SM4001PL-TPMSCT-ND/1793403
[Z945-ND]: http://www.digikey.com/product-detail/en/G6B-1114P-US-DC5/Z945-ND/148724