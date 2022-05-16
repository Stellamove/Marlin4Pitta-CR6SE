# Marlin4Pitta-CR6SE Firmware For CR-6 SE with Pitta

![GitHub](https://img.shields.io/github/license/Stellamove/Marlin4Pitta-CR6SE)

Marlin4Pitta-CR6SE is an optimized firmware for CR-6 SE with Pitta.

## Installing Marlin4Pitta-CR6SE
To install Marlin4Pitta-CR6SE on CR-6 SE you’ll first need to Download Marlin4Pitta-CR6SE, then use an IDE to Compile the Marlin4Pitta-CR6SE into a binary form and Upload it to your board. Download Marlin4Pitta-CR6SE source code on the [Github page](https://github.com/Stellamove/Marlin4Pitta-CR6SE)

![download](https://user-images.githubusercontent.com/96027590/145907300-a39be774-6594-4594-b73b-d7e76439e0f6.jpg)

## Building Marlin4Pitta-CR6SE
To build Marlin4Pitta-CR6SE you'll need [Visual Studio Code](https://code.visualstudio.com/) and [PlatformIO](https://docs.platformio.org/en/latest//integration/ide/index.html#platformio-ide). PlatformIO extension turns Visual Studio Code into a complete IDE for compiling and developing Marlin4Pitta-CR6SE.

![platformio](https://user-images.githubusercontent.com/96027590/145910073-1413379d-7f93-4516-ac42-30f6231ab456.jpg)

### 1. Install Visual Studio Code
Visit the [Visual Studio Code](https://code.visualstudio.com/) page to download and install the latest Visual Studio Code for your particular platform.

### 2. Install PlatformIO extension
Head over to the [Get PlatformIO IDE](https://platformio.org/install/ide?install=vscode) page to learn how to install PlatformIO IDE in VSCode.

### 3. Open Marlin4Pitta in Visual Stdio Code with PlatformIO
You can open Marlin in Visual Studio Code by use the Open Folder command in the Visual Stdio Code's File menu.

### 4. Build, Clean
Use the bottom Status Bar icons to build or clean.

![build](https://user-images.githubusercontent.com/96027590/145912771-bc4068ba-0bb7-4cd6-96e2-744c8dde9246.jpg)

## Upload firmware to CR-6 SE
CR-6 SE require the firmware.bin file to be copied onto the onboard SD card, and then you must reboot the printer to complete the install. Firmware binary file is located in the ".pio/build/(your target board)/" folder.

![firmware](https://user-images.githubusercontent.com/96027590/145913563-e3164dec-4648-4d95-b00d-e1b66b650789.jpg)

1. Prepare SD card formated with MBR, FAT32 and 4096 allocation size.
2. Copy the firmware binary file to the root of the card.
3. Ensure that the name of the file was not previously used to update the 3D printer.
4. Turn off the 3D printer, disconnect any USB cable and insert the SD card.
5. Turn on the 3D printer, the upload firmware process will start automatically.
6. The LCD will be blank until the upload is finished (about 15 seconds).
7. If you are uploading from the original firmware or other source, please restore defaults from LCD menu.

## Upload firmware to LCD of CR-6 SE
If you have uploaded the firmware of CR-6 SE, you must also upload the display firmware of the touch screen for CR-6 SE. You will find the instruction to upload and upload the DWIN_SET form [Configurations](https://github.com/Stellamove/Configurations/tree/master/config/examples/Creality/CR-6%20SE).
