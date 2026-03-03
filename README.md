# ZMK Config for Corne V3

Personal ZMK firmware configuration for Corne (crkbd) split keyboard with nice!nano v2 controllers.

## Building Firmware

Firmware is built automatically via GitHub Actions when you push to main.

1. Go to **Actions** tab
2. Click on the latest workflow run
3. Download the `firmware` artifact

## Flashing

1. Connect one half via USB
2. Double-tap the reset button to enter bootloader mode
3. Drag the appropriate `.uf2` file onto the USB drive:
   - `corne_left-nice_nano_v2-zmk.uf2` for left half
   - `corne_right-nice_nano_v2-zmk.uf2` for right half
4. Repeat for the other half

## Layers

- **Layer 0**: Default QWERTY
- **Layer 1**: Numbers and navigation (hold left thumb key)
- **Layer 2**: Symbols (hold right thumb key)
- **Layer 3**: Bluetooth controls (hold both thumb layer keys)

## Customizing

Edit `config/corne.keymap` to change your key layout.
Edit `config/corne.conf` to change keyboard settings.

## Resources

- [ZMK Documentation](https://zmk.dev/docs)
- [ZMK Keymap Editor](https://nickcoutsos.github.io/keymap-editor/)
