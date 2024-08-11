# Mini M OS with shader and other fixes

## Changes from "open" stock OS
- System settings:
    - Aspect ratio "auto"
    - Bilinear filtering "auto"
    - Show battery status "icon and text"
- Distribution.conf changes:
    - Remove `MagicX.glslp` default shader
    - Add `global.shaderset=none` to give back control to RA for shaders
- RetroArch config changes:
    - Show shaders in quick menu
    - Remember last shader dir
    - Set aspect ratio as "core provided"
    - Disable bilinear filtering
    - Disable threaded video
    - Enable notifications display
    - Enable logging, enable logging to file, enable log to file filestamps, set runtime logging directory
    - Disable RA quit on close content
    - Save config on exit
    - Disable menu sublabels
    - Clean up history
- SYSTEM live partition changes:
    - Replace stock shaders with newest version from official repository
- Permissions: Chmod -R 777 for the following directories:
    - `STORAGE/.config/distribution`
    - `STORAGE/.config/emulationstation`
    - `STORAGE/.config/retroarch`
    - `SYSTEM/usr/share/common-shaders`
- Device Tree Blob:
    - Replace with modded version by @shauninman

