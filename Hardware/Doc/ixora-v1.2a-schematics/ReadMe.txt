Toradex Ixora Carrier Board Schematics
---------------------------

This zip file contains the Schematics for the Ixora
If you have any question contact our support at: 
support@toradex.com


Change Log
----------

- Initial Release: Ixora V1.0A
  Release Date: 22 November 2013

- Design Revision: Ixora 1.1A
  Hardware_Architecture.SchDoc: Block diagram has been updated.
  Power_Supply.SchDoc: Comments near the capacitors C7 to C12 have been updated.
  Power_Switch.SchDoc: MOSFETs T8 and T10 have been replaced with new parts (Diodes Inc, Part Number: DMP4015SSS-13). 
              Zener Diodes D14 and D16 (OnSemi, Part Number: MM3Z20VT1G) have been added.
              Inductor L4 and current sense resistor R9 have been changed to increase 3.3V power supply rating.
              WAKE1_MICO# signal has been pulled up to 3.3V using R146, instead fo 3.3V_SW.
  RTC.SchDoc: Components related to EEPROM circuit (IC14, C97, R92, R93, R94, R95) have been marked as not assembled. 
              Diodes D3 and D4 have been replaced with single Diode D3.
  SDCard.SchDoc: Apalis MMC interface has been used (4 bit mode) in place of Apalis SD interface. 
              Micro SD Card holder X10 has been replaced with new connector (Wurth, Part Number: 693071010811). 
              NOTE 2 has been added.
  AudioSchDoc: Biasing circuit has been added to the microphone input. 
  Camera_Interface.SchDoc: MIPI CSI Connector X28 has been added.
              Recovery mode jumper JP4 has been added.
  RGB_Display.SchDoc: Capacitive touch connector X24 has been added.
  LVDS.SchDoc: Apalis I2C2 signals have been connected to the connector X19, pins 36 and 38.
  CAN.SchDoc: CAN bus termination resistors R107, R108, R113, R114 and capacitors C112, C121 have been marked as not assembled.
  Extension.SchDoc: MXM3_180, MXM3_186 and MXM3_176 have been connected to UART2/3_RS232_FOFF#, FACTORY_DEFAULT# and PCIE_WDISABLE#_R signals respectively.
              MXM3_188 and MXM3_178 have been used to control LED_4 (LED_4_GREEN and LED_4_RED) respectively.
  USB.SchDoc: USB power switch (IC7) has been replaced with higher current rating USB switch (TI, Part Number:TPS2066CD, overcurrent limit 1A).
  USB.SchDoc and PCI_Express.SchDoc: USB2 and USB3 interface connections have been swapped to ensure compatibility with the Apalis TK1 module. 
              As default assembly, USB2 has been connected to the PCIe connector and USB3 has been connected to the connector X7 (USB 1 connector).
  Release Date: 16 March 2017

- Updated support email address in the readme file.
  Release Date: 15 May 2017

- HDMI.SchDoc: NOTE 3 has been added.
  Release Date: 27 July 2017

- PowerSwitch.SchDoc: NOTE 4 has been added.
  Release Date: 16 April 2018

- Design Revision: Ixora 1.2A
  Hardware_Architecture.SchDoc: Block diagram has been updated.
  Power_Supply.SchDoc: To improve EMI/ESD performance of the board CHASSIS_GND has been implemented.
  Power_Switch.SchDoc: New DC-DC Buck / Step-down regulators have been used, inorder to increase the output power of the 3.3V and 5V_SW power supply.
              SH1 and SH2 pins of the tactile switches (SW1, SW2) are connected to CHASSIS_GND.
  RTC.SchDoc: New EEPROM (AT34C02D-XHM-B, TSSOP-8 package) has been added.
  USB_Connectors.SchDoc: New microUSB connector has been used (Hirose, ZX62-AB-5PA(31)).
	      USB connectors (X7, X8, X9) shield circuit has been updated to improve EMI/ESD performance.
  SDCard.SchDoc: SD card holder S1, S2 pins are now connected to GND. 
              ESD protection diode (D4) has been added to MMC_CD1 and MMC_CD2 signals.
              SD card pull-up resistors (R60, R61, R62, R63, R64) are not assembled by default.
              Load switch (IC22; Microchip MIC94070YMT-TR) has been added to control SD card power.
              MXM3_148/MMC1_D4 pin is used enable/disable the load switch for SD Card power.
              MXM3_158/MMC1_D7 pin is used enable/disable the load switch for CAN1 interface power.
  Ethernet.SchDoc: New RJ45 connector (X11; BEL Fuse A829-1J1T-KM; -40C to 100C operating temperature range) has been used.
              Components L20, C72, C73, R73, R74, R74, R76 are not assembled by default. NOTE 5 has been added in the schematic page.
              RJ45 connector (X11) shield circuit has been updated to improve EMI/ESD performance.
  AudioSchDoc: Capacitors C85 and C86 value has been changed to 4.7uF/10V.
  HDMI.SchDoc: New Voltage Level Shifter and ESD protection solution (IC9; Nexperia IP4786CZ32) has been used.
  CAN.SchDoc: Load switch ICs (IC18, IC19,IC20, IC21; Microchip MIC94070YMT-TR) have been added to control CAN1 and CAN2 interface power rails.
  SATA.SchDoc: Capacitors C164 (47uF) and C165 (47uF) have been added.
              MXM3_35/SATA1_ACT# pin has been used to enable/disable the load switch for CAN2 interface power.
  PCI_Express.SchDoc: Capacitors C162 (47uF) and C163 (47uF) have been added.
  Extension.SchDoc: MXM3_190 pin has been connected to shared pads resistors (R154, R155), as it may detect undesirable SD card detect interrupts. 
              SH1 and SH2 pins of the tactile switch (SW3) are connected to CHASSIS_GND.
  Mechanicals.SchDoc: New schematics page added for mechanical components. 
  Release Date: 08 October 2018

Important Disclaimer:
----------

Copyright © Toradex AG. All rights reserved. All data is for information purposes only and not
guaranteed for legal purposes. Information has been carefully checked and is believed to be
accurate; however, no responsibility is assumed for inaccuracies. Brand and product names are
trademarks or registered trademarks of their respective owners. Specifications are subject to
change without notice.


Trademark Acknowledgement:
----------

Brand and product names are trademarks or registered trademarks of their respective owners.
