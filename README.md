# Yamaha CR-2020 relay board LC-67183-1 CAD Reproduction
This is a modern CAD replica of the LC-67183-1 (relay) circuit board from the power supply of a Yamaha CR-2020 reciever.

![Finished Board](img/board_populated.jpg?raw=true "Finished Board")

[Front Detail](img/board_front.jpg?raw=true)

[Rear Detail](img/board_rear.jpg?raw=true)

## Summary
This project faithfully recreates the original board based on a sample LC-67183-1 board from a 1976 North American market CR-2020. A complete BOM is provided, including modern part substitutions where original parts may not be available.

Note that this replica doesn't *perfectly* recreate original board - some liberties were taken to make the design more suitable for modern components, and to make some practical changes.

AK user Jayfree also designed a replacement for the relay board, his is a modernized two-layer design instead of a reproduction of the original design. Available here: https://www.audiokarma.org/forums/index.php?threads/cad-new-yamaha-cr-2020-capacitor-board.912553/page-7#post-14397551 ([Photo](https://www.audiokarma.org/forums/index.php?threads/cad-new-yamaha-cr-2020-capacitor-board.912553/page-5#post-14284775))

Replica filter capacitor boards have been made as well:
1. [niclasf's board](https://foogadgets.blogspot.com/2020/05/yamaha-cr2020-repair.html) - to get one, contact niclasf on AK, or use his web store at https://www.facebook.com/foogadgets/
1. [jayfree's board](https://www.audiokarma.org/forums/index.php?threads/cad-new-yamaha-cr-2020-capacitor-board.912553/page-7#post-14397551) - ([Photo](https://www.audiokarma.org/forums/index.php?threads/cad-new-yamaha-cr-2020-capacitor-board.912553/page-4#post-14139270))

### Caution & Advice
* There are some small differences between model years, but as far as I can tell, this board should work for any model year. **Check your CR-2020's power supply carefully** before trying to use this reproduction board.
* At least 2oz copper is required for the PCB.
* The board's silkscreen includes very small text. JLCPCB will manufacture it, but the results aren't perfect. A PDF export of the silkscreen markings is included for reference.

In general, you should probably read this thread first: https://www.audiokarma.org/forums/index.php?threads/cad-new-yamaha-cr-2020-capacitor-board.912553/

### Acknowledgements
The author would like to thank AudioKarma users avionic, niclasf, and jayfree. Owe each of you a beer or 3. :)

## How-To
### Step 1: Order PCB
Recommend using JLCPCB (https://jlcpcb.com/).

Prepared gerber files for this board: [Gerbers, v1.0](https://github.com/flakzilla/cr2020-relay-board/raw/main/CR-2020%20relay%20board%20LC-67183-1/gerber%20zips/CR2020%20relay%20board%20LC-67183-1%20v1.0.zip)

Specify 1.6mm PCB thickness (this should be the default) and **2oz copper weight**. Thicker copper is mandatory due to high current passing through the relay.

### Step 2: Get Parts
BOM:
* [ODS Format](https://github.com/flakzilla/cr2020-relay-board/raw/main/CR-2020%20relay%20board%20LC-67183-1/BOM/BOM.ods)
* [Excel Format](https://github.com/flakzilla/cr2020-relay-board/raw/main/CR-2020%20relay%20board%20LC-67183-1/BOM/BOM.xlsx)

Carefully read and understand the notes in the BOM sheet, and check everything against your own CR-2020. It's recommended to recover and reuse the factory TO-92 transistors, if they're working.

### Step 3: Assemble
Populate the board.

Reference materials:
* [Board diagram](https://github.com/flakzilla/cr2020-relay-board/blob/main/CR-2020%20relay%20board%20LC-67183-1/reference/power%20supply%20c%20board%20diagram_fixed.png?raw=true) from the service manual, several typos and mistakes from the original manual have been fixed
* [PDF of PCB markings](https://github.com/flakzilla/cr2020-relay-board/blob/main/CR-2020%20relay%20board%20LC-67183-1/reference/markings%20diagram%20v1.0.pdf) since the silkscreen text on the board might be too small to read clearly
* [Some examples of TO-220 heatsinks](https://github.com/flakzilla/cr2020-relay-board/tree/main/CR-2020%20relay%20board%20LC-67183-1/reference/TO-220%20heatsink) that can be used for TR712/715

That's it, happy listening!

## License
This project is released under the terms of the Creative Commons Attribution + Noncommercial + ShareAlike (BY-NC-SA) license. https://creativecommons.org/licenses/by-nc-sa/2.0/

This project is distributed 'as-is' in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

