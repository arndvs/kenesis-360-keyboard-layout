# Programmer focused keyboard layout based on a modified Colemak Mod-DH layout

### Modifications from Colemak Mod-DH

1. The base layer focuses on easy use of symbols. The finger on the left hand that's used to open a symbol, is the same finger on the right hand to close it.
3. Additionally, the same fingers complete: Page Up & Page Down, Up Arrow & Down Arrow, Home & End, Left Arrow & Right Arrow, Escape & Tab, Back Space & Space, Delete & Enter. 
4. The alpha keys are based on the Colemak Mod-DH layout. However, the layout is modified to move the C and V letters to the right hand. This improves execution of commonly used 'ctrl+c' and 'ctrl+v' copy/paste.
5. The shift layer focuses on numbers as well as common git command macros. The numbers alternate left/right hand, similar to Dvorak. Odd numbers on the left hand and even numbers on the right hand. This keeps the most common numbers i.e. 1, 2, 3, 4 on the strongest fingers. It also allows quick back and forth typing on the strongest fingers. 

Base layer:
![Base layer:](https://i.imgur.com/HQCuEkJ.jpg)

Keypad:
![Keypad:](https://imgur.com/46Z6fKs.jpg)

Fn:
![Fn:](https://imgur.com/VxyEyHk.jpg)

Kinesis 360 Modification:
![Kinesis 360 Modification:](https://imgur.com/6NOFPeS.jpg)

Layer 4 (Shift):
![Layer 4 (Shift:](https://imgur.com/OXMoJje.jpg)



# ADV360-PRO-ZMK

## To build Firmware in GitHub Actions

### Setup

1. Fork this repo.
2. Enable GitHub Actions on your fork.

### Build firmware

1. Push a commit to trigger the build.
2. Download the artifact.

## To build Firmware locally using a container

### First run

Note: Either Podman or Docker is required, Podman is preferred if both are present.

1. Execute `make all`.
2. Check the `firmware` directory for the latest firmware build.

### Subsequent runs

If the only file you have changed is `config/adv360.keymap`, execute `make build` and check the `firmware` directory for the latest firmware build.

If you have changed other files in the `config` directory (such as `config/west.yml`) you will need to execute `make all` to rebuild the Docker image as well as the firmware.

### Flash firmware

Resources can be found on Kinesis.com
https://kinesis-ergo.com/support/kb360pro/#firmware-updates
https://kinesis-ergo.com/support/kb360pro/#manuals
