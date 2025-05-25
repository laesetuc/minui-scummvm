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

**Default key bindings:**
- A button / L1 button = Left click
- B button / R1 button = Right click
- X button = Period (Skips a line of dialogue)
- Y button = P (Pick Up)
- Start button = Open ScummVM menu
- Select button = Escape (Pause game)
- R2 button (hold down + dpad) = Fine mouse movement
- Menu button = opens NextUI menu

- NextUI/MinUI save states will not work - this is a limitation of ScummVM. Instead, open up the ScummVM menu and use the Save/Load functions there.
- NextUI suspend and sleep is working - power button behaves as per normal.
- CPU is set to normal by default, to overcome choppy audio
- Use NextUI Menu > Emulator > RetroPad mapping to remap buttons to ScummVM/mouse/keyboard controls

## Work in Progress / Known Issues

- Create ScummVM launcher shortcut
- Auto-detect games
- Is it possible to map MinUI/NextUI shortcuts to ScummVM shortcuts?  Perhaps quick save/quick load

### Tips

- pablodaniel : you can avoid music crackling if you set a fixed cpu speed in the nextui frontend menu, either powersave or normal
- pablodaniel : emulator options > timing > framerate cap to 60 hz also seems to help with the crackling

## Acknowledgements

- [MinUI](https://github.com/shauninman/MinUI) by Shaun Inman
- [PakUI](https://github.com/tenlevels/PakUI) project for the libretro core.

## License

This project is released under the MIT License. For more information, see the [LICENSE](LICENSE) file.
