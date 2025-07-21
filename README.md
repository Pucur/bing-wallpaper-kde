Bing Wallpaper for KDE Plasma
=================================

Information
-----------
A script which downloads the latest picture of the day from Bing.com and saves
it to a directory.

The script was tested on:

- Arch 6.15.7-arch1-1 KDE Plasma

How to use?
-----------
* Just run the **bing-wallpaper.sh** script from the terminal. The script will
download today's bing image.
* To see available options run the sript with the `--help` flag:

```
$ ./bing-wallpaper.sh --help
Usage:
  bing-wallpaper.sh [options]
  bing-wallpaper.sh -h | --help
  bing-wallpaper.sh --version

Options:
  -f --force                     Force download of picture. This will overwrite
                                 the picture if the filename already exists.
  -s --ssl                       Communicate with bing.com over SSL.
  -b --boost <n>                 Use boost mode. Try to fetch latest <n> pictures.
  -q --quiet                     Do not display log messages.
  -n --filename <file name>      The name of the downloaded picture. Defaults to
                                 the upstream name.
  -p --picturedir <picture dir>  The full path to the picture download dir.
                                 Will be created if it does not exist.
                                 [default: $HOME/Pictures/bing-wallpapers/]
  -r --resolution <resolution>   The resolution of the image to retrieve.
                                 Supported resolutions:
                                 UHD 1920x1200 1920x1080 800x480 400x240
  -w --set-wallpaper             Set downloaded picture as wallpaper (Only mac support for now).
  -h --help                      Show this screen.
  --version                      Show version.
```

Configuration on KDE
-----------------------
**TL;DR:**

* To install KDE background slideshow, in the terminal run:

```
$ git clone https://github.com/Pucur/bing-wallpaper-kde.git
```

* Change the background properties to use the new slideshow.

**How to register bing-wallpaper.sh or bing-random-pic.sh to run regularly.**

* Startup programs:
  * From HUD, search for startup applications.
  * Add **bing-random-pic.sh** or **bing-wallpaper.sh**.
