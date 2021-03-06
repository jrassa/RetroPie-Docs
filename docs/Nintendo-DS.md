***
![nds](https://cloud.githubusercontent.com/assets/10035308/12213354/eab79344-b633-11e5-805b-7d1a93fa44dd.png)
***
The Nintendo DS is a handheld video game console that was released by Nintendo in 2004. The DS stands for Dual Screen.
***

| Emulator | Rom Folder | Extension | BIOS |  Controller Config |
| :---: | :---: | :---: | :---: | :---: |
| [DraStic](http://drastic-ds.com/) | nds | .nds .zip | nds_bios_arm7.bin (optional), nds_bios_arm9.bin (optional), nds_firmware.bin (optional) | /opt/retropie/configs/nds/drastic/config/drastic.cfg |
| [lr-desmume](https://github.com/libretro/desmume) | nds | .nds .zip | bios7.bin (optional), bios9.bin (optional), firmware.bin (optional) | /opt/retropie/configs/nds/retroarch.cfg |

## Emulator: [DraStic](http://drastic-ds.com/)

Note that while DraStic may run very well, it is currently experimental beta software. Any games that use the microphone will only create noise and will not use a real microphone, Also any games in "bookmode" (e.g Brain Training) will always play rotated at 90 degrees and cannot be rotated in Drastic. 

## BIOS

The default installation of DraStic includes simulated BIOS files that will work in most cases. Actual BIOS files (listed above) can be added to
```
/opt/retropie/configs/nds/drastic/system
```

## ROMS
Accepted File Extensions: **.nds .zip**

Place your DS ROMs in 
```
/home/pi/RetroPie/roms/nds
```

## Controls

### DraStic Controls

Add custom controls using the DraStic GUI (by pressing RIGHT ANALOG RIGHT or DOWN ANALOG RIGHT (in some case) or "m" key on the keybord), or by editing
```
/opt/retropie/configs/nds/drastic/config/drastic.cfg
```

## Emulator: [lr-desmume](https://github.com/libretro/desmume)

Note that lr-desmume is very experimental and lags quite a bit even with an overclocked RPI 2/3.

## BIOS

lr-desmume can load BIOS file: **bios7.bin**, **bios9.bin** and **firmware.bin**

Place your bios7.bin, bios9.bin and firmware.bin BIOS file in
```
/home/pi/RetroPie/BIOS
```

## ROMS
Accepted File Extensions: **.nds .zip**

Place your DS ROMs in 
```
/home/pi/RetroPie/roms/nds
```

## Controls

### lr-desmume Controls
lr-desmume utilises Retroarch configurations

Add custom retroarch controls to the retroarch.cfg file in
```shell
/opt/retropie/configs/nds/retroarch.cfg
```
For more information on custom RetroArch controls see: [RetroArch Configuration](RetroArch-Configuration)

![nintendo_ds_diagram](https://cloud.githubusercontent.com/assets/10035308/16599645/7f549f56-42c0-11e6-88a8-3acda5287da3.png)