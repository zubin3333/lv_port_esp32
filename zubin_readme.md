# Notes by Zubin

## How to build and flash to esp32
First add esp-idf to path by running the following command (this is temporary so have to run every time you develop):
```
. $HOME/esp/esp-idf/export.sh
```

If you just want to build:
```
idf.py build
```

If you want to build and flash:
```
idf.py -p /dev/tty.SLAB_USBtoUART flash
```

Had to play around a lot to get the colors right using the esp config system:
```
idf.py menuconfig
```
These get saved to the sdkconfig file in the root directory, it seems like this isn't usually commited, but I commited it anyway because it took so long to optimise the setting for the ili9341.
