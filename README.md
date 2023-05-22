## [2.0.3] 2023-05-22

SOFTSHQIP.COM
Special thanks to @fidof1 

### BREAKING CHANGES (These changes will break your data on device, please make sure made a backup, also you can not use your old settings on this release but only can restore user data)

#### Added
- [firmware] Open/Close Button support
- [firmware] Logging Open/Close Button
- [firmware] the VERSION string is now defined at the beginning of main.cpp
- [firmware] #218 Added latching relay support
- [firmware] #189 Flash layout changed to 2MB Firmware / 2MB SPIFFS Data
- [firmware] Support for RDM6300 RFID readers (125kHz, UART) #163
- [firmware] debug firmware for debugging purposes
- [tools] executables for tools (no longer need to have node js and gulp for web ui development - **only lightly tested**) 
- [firmware] LED_BUILTIN lights up while wifi connected and flashes when it waits for wifi
- [webui] IP address choice option in AP mode
- [webui] favicon.ico
- [tools] websocket emulator can now store new configuration temporarly
- [firmware] log for firmware update #152
- [webui] Expired access attempts logged as "Expired"

#### Fixed
- [firmware] UART Monitor speed
- [firmware] avoid double Serial.begin
- [firmware] removing redundant terminating null character
- [firmware] fix the loadconfiguration loop
- [firmware] not able to connect MQTT server #157
- [firmware] a MQTT message typo #157
- [webui] some breaks on web pages 
- [webui] usage of !important CSS rule
- [firmware] #191 relay type inversion
- [firmware] #190 Increase PN532::WaitReady debug level
- [firmware] validuntil is being ignored #151
- [firmware] the boot loop when ssid is empty on configuration file (actually more a workaround than a fix) #154 

#### Changed
- [firmware] unify output format debug print of PICC
- [firmware] Improve onWsEvent() function
- [build] Change release type to a zip file (was tar.gz before)
- [webui] scrollbar on desktop screens (now hidden)
- [webui] sidebar colors (i hope you like it, standart bootstrap color)
- [webui] sanity check for firmware update file #152
- [firmware] lock MFRC522 library to version 1.4.1
