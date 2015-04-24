# MinimOSD Flashpack

**Please note: MultiWii is currently the only supported firmware in this package.
I will be trying to add more in the near future.**

## Included OSDs

* MW OSD
* KV Team OSD

## OSD Hardware Support

* MinimOSD

## Instructions

1. Install drivers if necessary
  * Currently only the win32 and win64 packages contain FTDI drivers
1. If you installed drivers, please restart your computer
1. Connect the FTDI adapter to the MinimOSD
1. Connect the FTDI adapter to your computer
1. Launch the included copy of Arduino (it contains all of the firmware files!)
  * The Arduino application is located the in root folder of this package
1. Prepare to flash the MinimOSD
  1. *Tools > Board > MinimOSD*
  1. *Tools > Serial Port > [Select the correct COM port]*
  1. *Tools > Programmer > FTDI Adapter (5V)*
1. Flash the EEPROM\_Clear program
  1. *File > Examples > MinimOSD > EEPROM\_Clear*
  1. *File > Upload*
  1. After a successful upload, wait a few moments and the status LED on the MinimOSD should go solid
1. If the upload fails, or the LED does not go solid after 30 seconds:
  * Make sure that the correct COM port is selected in *Tools > Serial Port*
  * Make sure that the FTDI adapter is set to 5V
  * Make sure that the FTDI adapter is securely connected to the MinimOSD board
1. Flash the OSD firmware
  1. *File > Examples > MinimOSD > MW\_OSD > MW\_OSD\_R1.3\_SP2 (or another firmware of your choice)*
  1. *File > Upload*
1. Once both EEPROM\_Clear and the firmware have been successfully flashed, close Arduino
1. Locate and launch the GUI that matches the firmware that you flashed
  * The GUI files are located in the root folder of this package
  * Unfortunately, a few GUIs are missing on certain OSs because they were not included in the original OSD package
1. The videos below will show you how to configure your MinimOSD using the GUI
1. Before closing the GUI, do not forget to disconnect the COM port!

## Video Tutorials

- [MultiWii + MinimOSD (Painless360)](https://www.youtube.com/watch?v=F1IjdudOrgM)
- [Naze32 + MinimOSD (Mochaboy RC)](https://www.youtube.com/watch?v=ikKH_6SQ-Tk)
- [Naze32 + MinimOSD (Painless360)](https://www.youtube.com/watch?v=Bdki9lIv31I)
- [MinimOSD Setup (Mochaboy RC)](https://www.youtube.com/watch?v=-myOXGkvksY)
