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

