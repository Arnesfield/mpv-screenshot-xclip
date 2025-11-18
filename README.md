# mpv-screenshot-xclip

Take a screenshot and use `xclip` to copy the image file to clipboard.

## Requirements

- Requires [mpv](https://mpv.io/).
- Requires `file` in `PATH` to get the image file mime type.
- Requires `xclip` in `PATH` to copy image files to clipboard.

## Install

1. Download [`screenshot-xclip.lua`](screenshot-xclip.lua) and place it under the `scripts` directory of your mpv config (e.g., `~/.config/mpv`).

   Or run the following to download it:

   ```sh
   wget github.com/Arnesfield/mpv-screenshot-xclip/raw/main/screenshot-xclip.lua
   ```

2. Add the following keybindings to `input.conf` to replace the default screenshot keybindings:

   ```conf
   s script-message screenshot-xclip
   S script-message screenshot-xclip video
   ctrl+s script-message screenshot-xclip window
   alt+s script-message screenshot-xclip each-frame
   ```

## License

Licensed under the [MIT License](LICENSE).
