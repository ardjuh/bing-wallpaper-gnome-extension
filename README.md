# Fork
This is a fork from [Bing wallpaper of the day](https://github.com/neffo/bing-wallpaper-gnome-extension). This fork probably won't be updated frequently and as of now has the wrong metadata.

# GNOME Shell extension - Youversion votd image

Bring some color to your GNOME desktop by syncing your desktop and lockscreen wallpapers with today's Youversion's verse of the day image with this extension. The intention of this extension is to just do what it needs to do and stay out of your way, with a few optional features to improve quality-of-life.

## Features

* Automatically sets the Youversion [Verse of the Day image](https://www.bible.com/verse-of-the-day) as both lock screen and desktop wallpapers
* Only attempts to download wallpapers when they have been updated - doesn't poll continuously
* Shuffle/randomise wallpapers at adjustable intervals (including from your stored Bing images)
* Image gallery to view, select and curate stored images
* Optionally delete old images after a week, or you can keep (and curate) them forever
* Override the lockscreen blur (NEW: lockscreen blur is now dynamic!)
* Language support: English (en), German (de), Dutch (nl), Italian (it), Polish (pl), Chinese (zh_CN, zh_TW), French (fr_FR), Portuguese (pt, pt_BR), Ukrainian (uk), Russian (ru_RU), Spanish (es), Korean (ko), Indonesian (id), Catalan (ca), Norwegian Bokmål (nb) & Nynorsk (nn), Swedish (sv), Arabic (ar), Hungarian (hu), Japanese (ja), Czech (cs_CZ), Finnish (fi_FI) and Turkish (tr) - a HUGE thanks to the translators
* Image preview in menus & ability to manually set wallpapers individually or copy image to clipboard
* A selection of different theme-aware indicator (tray) icons to choose (or hide it completely)

## TODO

* Scale image so it fits nicely on the screen
* Remove all requests to bing
* Update metadata.json

## Requirements

GNOME 3.36+ or 40+ (Ubuntu 20.04 LTS or later, older versions of the extension work with 3.18+, but are no longer supported).

## Install

install directly to your GNOME extensions directory (useful if you want to hack on it)

```
mkdir ~/Desktop/source
cd ~/Desktop/source
git clone git@github.com:ardjuh/bing-wallpaper-gnome-extension.git
cd bing-wallpaper-gnome-extension
sh install.sh
```

## Enable debug logging

Enable debug logging through the exptension preferences 'Debug options' tab or if unable to open preferences you can enable debugging using dconf-editor with this command:
```
GSETTINGS_SCHEMA_DIR=$HOME/.local/share/gnome-shell/extensions/BingWallpaper@ineffable-gmail.com/schemas dconf-editor /org/gnome/shell/extensions/bingwallpaper/
```

Please include logs from your journal when submitting bug notices (make sure nothing sensitive is included in the text!).

## Screenshots

### Image gallery

![Settings](/screenshot/settings5.png)

### Preferences

![Settings](/screenshot/settings.png)
![Settings](/screenshot/settings2.png)
![Settings](/screenshot/settings3.png)
![Settings](/screenshot/settings4.png)


### Lockscreen blur control
From left to right: 
* no blur/no dimming
* slight blur/default dimming
* default blur/default dimming
![Blur example](/screenshot/blurexample.jpg)

## Toss a coin to your coder

Do you like this extension and want to show that you appreciate the work that goes into adding new features and keeping it maintained? Please consider buying me a coffee on [GitHub Sponsors](https://github.com/sponsors/neffo) or on [Flattr](https://flattr.com/@neffo). This is for the original creater neffo, not me.

## Disclaimer

This extension is unofficial and not affiliated with Bing or Microsoft in any way. Images are protected by copyright, and are licensed only for use as wallpapers.

## Special Thanks

This extension is based on the NASA APOD extension by [Elinvention](https://github.com/Elinvention)
and inspired by Bing Desktop WallpaperChanger by [Utkarsh Gupta](https://github.com/UtkarshGpta). Lockscreen blur code is based on [Pratap-Kumar's extension](https://github.com/PRATAP-KUMAR/Control_Blur_Effect_On_Lock_Screen). I'd like to give a special shout out to those who have [contributed code and translations](https://github.com/neffo/bing-wallpaper-gnome-extension/graphs/contributors) as well as everyone who has reported bugs or provided feedback and suggestions for improvements. Also, thanks to Microsoft for this great API and wallpaper collection.

## License

This extension is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
