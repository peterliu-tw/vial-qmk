# How to build using vial-qmk

I use [**vial-qmk**](https://github.com/vial-kb/vial-qmk) instead of the upstream [**qmk-firmware**](https://github.com/qmk/qmk_firmware) for one primary reason:  
> The [VIA web configurator](https://www.usevia.app/) does not currently support the Avalanche keyboard.  

VIA support requires the keyboard definition to be merged into the official VIA repository. Until someone contributes and pushes the Avalanche layout upstream, it will not be available in the VIA web configurator.  

In the meantime, [**VIAL** configurator](https://get.vial.today/) provides equivalent functionality with immediate support, making it the practical choice for Avalanche users.

The downside of VIAL-QMK is it use a lot of EEPROM size. So lots feature are disabled.


To build:
``` bash
git clone https://github.com/peterliu-tw/vial-qmk.git
cd ./vial-qmk
qmk compile -kb avalanche/v4 -km vial
```
Visit https://docs.qmk.fm/ for more detailed setup.

# How to flash
Get QMK Toolbox and google on how to use it.



# How to Configure keymap 
1. User web configurator https://vial.rocks/ that overide the default keymap.
2. To change the default keymap, need recompile firmware.  Keymap for VIAL is here : `keyboards/avalanche/v4/keymaps/vial/keymap.c`



# Happy Creating the Best Programmer Keyboard
Again, visit https://docs.qmk.fm/ for a long list of QMK features that you can play with.
