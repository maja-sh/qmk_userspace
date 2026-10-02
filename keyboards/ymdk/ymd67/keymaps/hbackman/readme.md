# hbackman YMD67 layout

Based on the default YMD67 layout, with the following changes:

- Right Ctrl is a third `MO(1)` key.
- `Esc` is `QK_GESC`: `Shift` + `Esc` is `~` and `Cmd` + `Esc` is `Cmd` + `` ` ``.
  `GRAVE_ESC_ALT_OVERRIDE` keeps `Cmd` + `Option` + `Esc` (Force Quit) working.
- `Fn` + `Esc` is `` ` ``.
- `Fn` + `\` is `QK_BOOT`, since `Fn` + `Esc` is no longer the bootloader key.
- `Fn` + `Tab` pastes the clipboard wrapped in a fenced code block:
  ```` ``` ````, `Shift` + `Enter`, `Cmd` + `V`, `Shift` + `Enter`,
  ```` ``` ````. Uses `Shift` + `Enter` so chat inputs don't submit early, and
  `Cmd` + `V`, so it assumes macOS.
- `Fn` + `Shift` + `Tab` types an empty fenced code block and moves the cursor
  to the blank line inside it.

Holding `Esc` while plugging the keyboard in also enters the bootloader
(bootmagic), which is the fallback if the firmware is unresponsive.
