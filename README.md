# ardux-keyboard

## Changes from the 40p ardux
* Miryoku instead of 40p ardux ansi
    * MIRYOKU_CLIPBOARD=WIN
    * MIRYOKU_NAV=VI
    * Doesn't include additional features of `Boot`, `Tap`, `Extra`, `Base`, `Opp`, `Cur` 
* UK keycodes
    * `KC_BSLS -> KC_NUBS`
    * `KC_HASH -> KC_NUHS`
    * `KC_PIPE -> S(KC_NUBS)`
* built with
    ```bash
    rm -rf ../../.build/* && qmk -v compile \
        -e ARDUX_SIZE=40p \
        -e ARDUX_HAND=left \
        -e ARDUX_REMIX=yes \
        -e RGBLIGHT_ENABLE=yes \
        -e OLED_ENABLE=no \
        users/ardux/layout/crkbd_r2g_40p.json
    ```