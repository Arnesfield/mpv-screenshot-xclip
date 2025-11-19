# mpv-screenshot-xclip

Take a screenshot and use `xclip` to copy the image file to clipboard.

## Requirements

- Requires [mpv](https://mpv.io/).
- Requires `file` in `PATH` to get the image file mime type.
- Requires `xclip` in `PATH` to copy image files to clipboard.

## Install

1. Download the following files to their appropriate directories under your mpv config (e.g., `~/.config/mpv`):

   [`screenshot-xclip.lua`](screenshot-xclip.lua) - Save to `scripts` directory.

   ```sh
   wget github.com/Arnesfield/mpv-screenshot-xclip/raw/main/screenshot-xclip.lua
   ```

   [`screenshot-xclip.conf`](screenshot-xclip.conf) - (optional) Save to `script-opts` directory.

   ```sh
   wget github.com/Arnesfield/mpv-screenshot-xclip/raw/main/screenshot-xclip.conf
   ```

1. Add the following keybindings to `input.conf` to replace the default screenshot keybindings:

   ```conf
   s script-message screenshot-xclip
   S script-message screenshot-xclip video
   ctrl+s script-message screenshot-xclip window
   alt+s script-message screenshot-xclip each-frame
   ```

## Config

List of configuration options ([`screenshot-xclip.conf`](screenshot-xclip.conf)).

### disable_osd_messages

Disables OSD messages by log level. Comma-separated values of: `info`, `error`

Example:

```conf
disable_osd_messages=info,error
```

## License

Licensed under the [MIT License](LICENSE).
