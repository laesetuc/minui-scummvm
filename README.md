# minui-scummvm
Experimetal ScummVM emulator for NextUI

## Requirements

This pak is designed for and tested with the following MinUI Platforms and devices:

- `tg5040`: Trimui Brick (formerly `tg3040`)

## Installation

1. Mount your MinUI SD card.
2. Download the latest [release](https://github.com/laesetuc/minui-scummvm/releases) from GitHub.
3. Copy the zip file to the correct platform folder in the "/Emus" directory on the SD card.
4. Extract the zip in place, then delete the zip file.
5. Confirm that there is a `/Emus/$PLATFORM/SCUMMVM.pak/launch.sh` file on your SD card.
6. Unmount your SD Card and insert it into your MinUI device.

Note: The platform folder name is based on the name of your device. For example, if you are using a TrimUI Brick, the folder is "tg5040". Alternatively, if you're not sure which folder to use, you can copy the .pak folders to all the platform folders.

## Usage

1. Create the /Roms/ScummVM (SCUMMVM)/ directory if you haven't already.
2. Copy your game into this directory e.g. /Roms/ScummVM (SCUMMVM)/The Secret of Monkey Island/
3. Create a shortcut file e.g. /Roms/ScummVM (SCUMMVM)/The Secret of Monkey Island/The Secret of Monkey Island
4. Edit the shortcut file and insert approrpriate the ScummVM ID from the [ScummVM Compatibility list](https://www.scummvm.org/compatibility/)
e.g. scumm:monkey

### Controls
- B button / L1 button = Left click
- R1 button = Right click
- A button = Cancel
- Start button = ScummVM menu
- Menu button = opens NextUI menu
- Suspend and sleep seem to work
- NextUI/MinUI save states will not work - this is a limitation of ScummVM. Instead, open up the ScummVM menu and use the Save/Load functions there.

### Tips

- pablodaniel : if you set a fixed cpu speed in the nextui frontend menu, either powersave or normal
- pablodaniel : emulator options > timing > framerate cap to 60 hz also seems to help with the crackling

## Work in Progress / Known Issues

- Sound can get a little choppy in parts
- Key bindings should be remapped to be friendlier (maybe A = left click, B = right click)
- Is it possible to map MinUI/NextUI shortcuts to ScummVM shortcuts?  Perhaps quick save/quick load
- Create ScummVM launcher shortcut
- Auto-detect games

## Acknowledgements

- [MinUI](https://github.com/shauninman/MinUI) by Shaun Inman
- [PakUI](https://github.com/tenlevels/PakUI) project for the libretro core.

## License

This project is released under the MIT License. For more information, see the [LICENSE](LICENSE) file.
