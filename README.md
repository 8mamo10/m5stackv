# m5stackv
Try V-Training.

## setup

### Firmware
- Connect M5StickV to Mac via USB type-C cable.
- Download firmware.
  - https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/M5StickV_Firmware_v5.1.2.kfpkg
- Install Kflash_GUI.
  - https://github.com/sipeed/kflash_gui/releases/download/v1.5.2/kflash_gui_v1.5.2_macOS.dmg
  - It didn't open with double click, so I lanuched it by the command below
  - `open /Applications/kflash_gui.app `
- Open Kflash_GUI and fill items.
  - Open File -> Select downloaded kfpkg file
  - Board -> Select M5StickV
  - Port -> Select M5Stack intf
- Press Download

### Boot file
- Download boot files.
  - https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/VTraining-Client-VerA02B01.zip
- Unzip VTraining-Client-VerA02B01.zip and copy files to SD card on Finder.
  - Reject SD card from M5StackV for this

### V-training
- I took picutres of 6 Pokemon cards from each of the 4 directions * 10 times, total 40 pictures for each pokemon.
  - About 240 pictures in total.
- Upload to V-Training.
  - http://v-training.m5stack.com/
- But it's too slow and every time it stops with an error in the middle...
  - I'll try again later.
- Finally, I could upload successfully, but got an error mail from V-Trainer.
```
CONTENT: Lake of Enough Train Dataset, Only 177 pictures found, but you need 180 in total.


Notice:
Image 8.jpg was removed for being too close to 7.jpg, hashdiff: 2

Image 9.jpg was removed for being too close to 7.jpg, hashdiff: 2

...
```
- It seems some of the pictures were too similar and didn't seem appropriate as input.
  - As a result of their elimination, the amount of data was insufficient.
- So next, I took the pictures of three Pokemon figures from various angles.
  - In case some pictures are eliminated as well, I took 50 picutres per one.
<img src="https://user-images.githubusercontent.com/562105/90320697-5c8f7400-df7e-11ea-97e6-32bf4a2b0a2c.png" width="320px">
- BTW, uploading to V-Training was quite fast at 5 am JST.

## Troubles
- Document says, `Power on ：Long press power button for 2 seconds`, but it does not work for my device.
  - I need to press Power on twice in a short time.

## References
- https://docs.m5stack.com/#/en/quick_start/m5stickv/m5stickv_quick_start
- https://docs.m5stack.com/#/en/related_documents/v-training
