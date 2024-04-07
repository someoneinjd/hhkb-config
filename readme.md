# HHKB Config

> Keyboard: Keychron Q60 MAX

## Keymap Changes

| Key                             | Old                       | New                       |
| ------------------------------- | ------------------------- | ------------------------- |
| <kbd>Delete</kbd>               | Delete                    | Backspace                 |
| <kbd>Fn</kbd> + <kbd>Ctrl</kbd> | Turn the backlight on/off | Ctrl                      |
| <kbd>Fn</kbd> + <kbd>Cmd</kbd>  | None                      | Turn the backlight on/off |

## Setup

1. Install QMK CLI

    ```shell
    # Homebrew (Mac)
    brew install qmk/qmk/qmk
    export PATH=/usr/local/opt/arm-none-eabi-binutils/bin:$PATH
    export PATH=/usr/local/opt/arm-none-eabi-gcc@8/bin:$PATH
    export PATH=/usr/local/opt/avr-gcc@8/bin:$PATH
    ```

2. Clone this repo

    ```shell
    git clone https://github.com/someoneinjd/qmk_firmware --recursive
    ```

3. Use QMK CLI to setup

    ```shell
    qmk setup
    ```

## Build

```shell
# Build & flash firmware 
make keychron/q60_max/ansi:default:flash

# Build only
make keychron/q60_max/ansi:default
```

[ref](./keyboards/keychron/q60_max/readme.md)
