# Collection of Atoto firmware files for unbricking
If you just want to update the firmware normally, you can find the files here: https://resources.myatoto.com/operation-guide/upgrade-instructions/index/  
This website is extremely buggy and the best way to access it is to use a phone or to use the developer tools in your browser to simulate a phone.  
Chrome: https://developer.chrome.com/docs/devtools/device-mode/#viewport

If your radio firmware isn't listed here, you'll have to contact Atoto support and ask for it. Make sure to ask specifically for the ISPBOOOT.BIN file. If they give it to you, please open a new issue in this repo with the link so it can be saved here.

Some files are split across multiple zip files to get around GitHubs max file size limit. For those files, download all the zip files in their respective folders then use software like 7zip to extract.

There's 2 different procedures that work for 99% of radios

Prerequisites:  
1. Get a USB drive or an SD card that you don't mind formatting. The smaller the better.
2. [Convert your drive from GPT to MBR](https://learn.microsoft.com/en-us/windows-server/storage/disk-management/change-a-gpt-disk-into-an-mbr-disk) then make a new partition formatted as FAT32
3. Make sure the firmware file is named exactly ISPBOOOT.BIN and copy it to your drive.
4. Completely eject the drive from your computer before unplugging it.  

Method 1:
1. Plug the flash drive or SD card into the front of the radio and turn it on.
2. While holding the home button, use a pen to press the reset button.
3. Keep holding the home button until a screen showing the old and new firmware versions pop up. When it appears you can let go of home. The update should finish in around 5 to 10mins

Method 2 (Requires that the illumination wire is connected and working. Read completely before doing this one):
1. Make sure the radio is completely off before beginning.
2. Plug the flash drive or SD card into the front of the radio.
3. Turn on power to the radio, wait about a second then turn your headlights on and back off 3 times. Wait until the screen or buttons dim a bit every time you turn them on.
4. The screen should go blank then show the old and new firmware versions and the update progress. The update should finish in around 5 to 10mins

Troubleshooting:
1. If the screen stays completely blank, try a different USB drive or SD card. You'll probably go through a lot before you find one that works.
2. If your illumination wire isn't hooked up, touching the wire to 12 volts will have the same effect as turning on the headlights. ***Be very careful if you do this. You can fry the radio or something in your vehicle if something goes wrong.***
