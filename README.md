# esp8266fatfs
A FatFs implementation for ESP8266

### What? ###

This implements the FatFs Generic FAT File System Module to work with the ESP8266 flash memory.

So you get a full working fat file system with folders and files.

The price you pay is (perhaps) heavy use of flashEraseSector and so an early death of your
ESP8266 flash memory chip. You have been warned! 

### Really that bad? ###

I don't know. Have to do some tests.

### Installation ###

A copy of preconfigured FatFs is included. Download, unzip to libraries, restart IDE and have a look at the examples.

To get a genuine FatFs copy go to http://elm-chan.org/fsw/ff/00index_e.html. You need to delete all diskio.* and replace it with this version files.

### Default operation ###

By default it reuses the space used by SPIFFS with the FatFs filesystem.

If it finds a ESP8266 with more than 4MB flash it will use that flash for file system.







