## Update TFT Firmware


TFT firmware updates are comprised of up to four elements:

1. The firmware binary (`BIGTREE_TFT*_V*.*.*.bin`). Example: `BIGTREE_TFT35_V3.0.26.1.bin`:
   - `BIGTREE_TFT_35`: model
   - `V3.0`: hardware version
   - `26.1`: software version
2. Fonts and Icons (`TFT*` folder):
   - `TFT*/font`: fonts
   - `TFT*/bmp`: icons
3. The config.ini file
4. **Optionally** a language file

Copy  the `BIGTREE_TFT*_V*.*.*.bin,the `TFT*` folder and the config.ini to the root of a blank SD card that is <8GB and formatted as FAT32:



![Copy](https://user-images.githubusercontent.com/54359396/96474405-0e734700-1233-11eb-9ecb-958a891e58d7.png)

**Optionally**, copy one or several language .ini file(s) from Copy to SD Card root directory to update/Language Packs [`Copy to SD Card root directory to update/Language Packs`](https://github.com/bigtreetech/BIGTREETECH-TouchScreenFirmware/tree/8963aed84c40a3b8daf2768a7feb37aeeab71996/Copy%20to%20SD%20Card%20root%20directory%20to%20update%20) folder onto the SD card. Doing so will allow you to switch between English and the uploaded language(s), using the corresponding Language function of the TFT. We recommend to upload the minimum amount of languages, to keep the memory usage low. The language .ini file can be edited to change the text shown on the TFT.

![Copy language](https://user-images.githubusercontent.com/54359396/98911362-c60f1800-24c4-11eb-95e6-e4f4dc64a9fb.png)


Place SD card with the `BIGTREE_TFT*_V*.*.*.bin`, the`TFT*` folder and the config.ini into the TFT's SD card reader and reset your TFT (or optionally - power cycle your printer) to start the update process.

<p align=center> ⚠️ Failing to update your icons &amp; fonts will result in missing icons and/or unreadable text ⚠️ </p>



## Update Process shown on TFT Screen

A successful update looks like this on the screen:

![Screenshot 2020-09-26 at 22 10 04](https://user-images.githubusercontent.com/54359396/94349526-5abcd400-0045-11eb-993a-afc5b241f4d7.png)

... and the name of the elements on the SD card changes to this:

![After Update](https://user-images.githubusercontent.com/54359396/94349755-dc156600-0047-11eb-9b1e-a1334bc5675f.png)

In case one or several parts of the update failed, an error will be shown. Follow the information on the screen to update the missing or outdated elements.

![Screenshot 2020-10-23 at 14 37 36](https://user-images.githubusercontent.com/54359396/97004894-002c7000-153e-11eb-9951-f493be46af3e.png)

<p align=center> ⚠️ Errors during the update can not be ignored and must be solved before using the TFT ⚠️ </p>

After the update is done and the files are renamed, it is possible to reuse them again. To do so, change the name of the element(s) to the pre-update name and start the update process again.

Remove the SD card from the TFT and restart the printer.




## Configuration

The Firmware can be configured using the **config.ini** file from:
[`Copy to SD Card root directory to update`](https://github.com/bigtreetech/BIGTREETECH-TouchScreenFirmware/tree/master/Copy%20to%20SD%20Card%20root%20directory%20to%20update)

### Editing configuration (config.ini) file

To edit the **config.ini** file follow the instruction here: [Detailed Instructions here](config_instructions.md)

### Updating Firmware Configuration

To update the Firmware configuration:

1. Edit the settings in **config.ini**.
2. Copy the **config.ini** file to the root of the SD card. (The SD card capacity should be less than or equal to 8GB and formatted as FAT32)
3. Insert the SD card into the TFT's SD card slot and restart the printer or press the reset buttion of the TFT.
4. The TFT will update and store the configuration from **config.ini** file.
5. Make sure to remove the SD card from the TFT and restart the printer.

The config.ini can be edited using a simple text editor (make sure to use UTF encoding) and uploaded again - without the need to upload the firmware or the TFT folder - as long as the firmware and the config.ini have the same version number.

## Customization

### Bootscreen and Icons

See [Customization guides](https://github.com/bigtreetech/BIGTREETECH-TouchScreenFirmware/tree/master/readme/) for detailed  information.
