## Summary
An ESP32 project.
Based on an ESP32 Dev Kit1
As of about Jun 15 2025
Device connects to a WiFi network with WiFi Manager
Device accept OTA update with Eligant OTA.

## Future features
Inrementaly add the following features.

1. Increment the verion
2. Will serve a web page which identifes the device as file name, PMD_BPM_wMQTT, and version number. The home web page will have a link to the update page.
3. The OLED display will report the status of the WiFi inilization. It will show the WiFi type such as softAP or STA. It will report the device MAC address. 
It will report the IP address of the SoftAP or the STA.


## Boot message as of V.0.1.94 

rst:0x1 (POWERON_RESET),boot:0x13 (SPI_FAST_FLASH_BOOT)
configsip: 0, SPIWP:0xee
clk_drv:0x00,q_drv:0x00,d_drv:0x00,cs0_drv:0x00,hd_drv:0x00,wp_drv:0x00
mode:DIO, clock div:1
load:0x3fff0030,len:4888
load:0x40078000,len:16516
load:0x40080400,len:4
load:0x40080404,len:3476
entry 0x400805b4
===================================
PMD_BPM_wMQTT  V.0.1.94 
Model: HW2_240421
20240421_USA4
Compiled at: Jun 15 2025 07:59:11
GNU Affero General Public License, version 3 
===================================
No saved WiFi credentials found.
*wm:AutoConnect 
*wm:Connecting to SAVED AP: VRX
*wm:connectTimeout not set, ESP waitForConnectResult... 
*wm:AutoConnect: SUCCESS 
*wm:STA IP Address: 192.168.1.247
Failed to save WiFi credentials.
Connected to WiFi!
Connecting to WiFi ....
                        Connected. IP Address: 192.168.1.247
LittleFS mounted successfully.
checking wifi...
                 connecting to WiFi...
                                       connected!
     


