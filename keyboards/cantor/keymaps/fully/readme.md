# 1 Modify the layout

1. https://config.qmk.fm
1. upload the json file C:\Users\onger\qmk_firmware\keyboards\cantor\keymaps\fully
1. Download the file to the same path

# 2 Convert to keymay.c

1. start QMK MYSYS
1. cd ./qmk_firmware/keyboards/cantor/keymaps/fully
1. qmk json2c fully.json -o keymap.c

# 3 Compile the firmware

1. qmk compile -kb cantor -km fully -j 8

# 4 Flash the firmwark

put keyboard half into flash mode
1. disconnect usb and aux cable
2. press the top left button on the left half or the top right button on the right half
3. qmk flash -kb cantor -km fully -j 8
4. reconnect the halves individually via usb
5. reconnect the aux cable and then the usb cable on the left half