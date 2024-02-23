This is the firmware for the rockon:
* https://fingerpunch.xyz/product/rock-on/
* https://discord.gg/ewS6xbCgPb
* https://github.com/sadekbaroudi/fingerpunch/tree/master/rock-on

Note that this is pre-configured without an OLED, though the keyboard does support an OLED. You will need to adjust the firmware to support.

For the `v1_cirque` branch, here is the command to build:
`west build --pristine -b nice_nano -- -DSHIELD=rockon -DZMK_CONFIG=/home/sadek/zmk-rockon/config -DZMK_EXTRA_MODULES="/home/sadek/cirque-input-module;/home/sadek/zmk-rockon"`  

Note that I tried to get it working on my personal board for the nice nano v2, but it didn't work unless I used nice nano as the board (-b nice_nano).

You should be running this from the zmk/app directory from the following repo and branch:
* `https://github.com/petejohanson/zmk/tree/feat/pointers-move-scroll`  

Please note that you should have cloned:
* `https://github.com/petejohanson/cirque-input-module`
* `https://github.com/sadekbaroudi/zmk-rockon`  
