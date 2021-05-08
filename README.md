# Goldrush
Achaea Prospecting script for Mudlet


## Installation Instructions

### Manual Installation
1. Download this repository as a ZIP by clicking the "Clone or download" button above
2. Unpack the ZIP somewhere...anywhere!
3. Open the mudlet packackage manager
4. Navigate to and install the "achaea-calendar.xml" script...wherever you put it...

### Automagic Installation
1. If you have a previous version installed, uninstall first via the package manager.
2. Copy the code below, paste into mudlet, press enter!

```
lua function d(_,f) if f~=getMudletHomeDir().."/Goldrush.xml" then return end installPackage(f) os.remove(f) echo('Installation Complete') end registerAnonymousEventHandler("sysDownloadDone","d") downloadFile(getMudletHomeDir().."/Goldrush.xml","https://thaisenachaeascripts.github.io/Goldrush/Goldrush.xml")
```

## Basic Usage

**GOLDRUSH** - Shows all of the available commands in the script

**GOLDRUSH SEARCH** is required to be run before you begin prospecting. This only needs to be done ONCE as all the potential lode locations will be maintained after you close mudlet.


## Features

- Automatic Prospecting of all potential lode rooms on MAINLAND, TUNDRA, and FISSURE
- Doesn't automatically walk to tundra or fissure, but can prospect once there.
- Pause/Resume functionality in the middle of prospecting run.
- Nice clean looking report after prospecting is complete
- Automatic logging to CFMG clan
- Automatic logging to Cyrene Discord

- QoL improvements while in a mine
  - Automatic walking from start to end of mine and vice versa
  - Automatic deployment of miners and legion
