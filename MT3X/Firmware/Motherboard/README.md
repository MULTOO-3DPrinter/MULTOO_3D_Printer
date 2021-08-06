





# Motherboard firmware update




This is a list of folders. The name of the folder represents the update date.

The files in the folder are `bin` files. 



## File name introduction


```
firmware_500.bin

The Z axis of the representative printer is 500mm.
```

```
firmware_500_high.bin

The Z axis of the representative printer is 500mm, and it is a high-temperature extruder version.
```


## Update steps

1. Turn off the printer.
2. Take out the TF card from the motherboard. If the TF card is lost, please prepare a TF card yourself. The minimum capacity of the TF card is 128M. The format of the TF card is FAT32.
3. Change the name of the file `firmware_xxx.bin` to `firmware.bin`.
4. If there is a residual file `FIRMWARE.CUR` in the TF card, please delete it.
5. Copy `firmware.bin` to the TF card.
6. Insert it on the motherboard in the electrical box.
7. Turn on the power to the electrical box. Wait about 20 seconds.

**Steps to see if the update is successful,**

When the screen is successfully connected to the printer, proceed as follows,
`Info` -> `Menu` -> `Settings` -> `Info`,
Check the time displayed in the System item. For example, the display content is,
`Marlin 2.0.6.1 (Aug 5 2021 00:06:10)`

If the time is different from the time of the previous version, it means the update was successful.
