# Programmer focused keyboard layout based on a modified Colemak Mod-DH layout

### Modifications from Colemak Mod-DH

1. The base layer is focused on symbols, where the finger on the left hand used to open, is the same finger on the right hand to close the symbol.
2. Additionally, the same finger on the left and right are used to complete: Page Up & Page Down, Up Arrow & Down Arrow, Home & End, Left Arrow & Right Arrow, Escape & Tab, Back Space & Space, Delete & Enter. 
3. The alphabet keys are based on the Colemak Mod-DH layout, which is slightly less of a jump from QWERTY than Drovak, but the layout is modified to move the C and V letters to the right hand to better execute the commonly used 'ctrl+c' and 'ctrl+v' copy paste.
4. On the shift layer there's numbers as well as common git command macros. 


Base layer:
![Base layer:](https://i.imgur.com/HQCuEkJ.jpg)



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
