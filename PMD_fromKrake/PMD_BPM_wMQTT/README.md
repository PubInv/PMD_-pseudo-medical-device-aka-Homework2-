## Summary
An ESP32 project.  
Based on an ESP32 Dev Kit1  
As of about Jun 15 2025, Device connects to a WiFi network with WiFi Manager and device accept OTA update with Eligant OTA.  

## Future features
Incrementally add the following features.

1. Increment the version
2. Serve a web page which identifies the device as FILE_NAME (PMD_BPM_MQTT) and version number. The home web page will have a link to the update page.
3. The OLED display will report the status of the Wi-Fi initialization. It will show the Wi-Fi type such as soft AP or STA. It will report the device MAC address. 
It will report the IP address of the Soft AP or the STA.
4. Correct the serial monitor messages that appear to be incorrectly saying Wi-Fi credentials not saved. 


## Boot message as of V.0.1.94  
```
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
     

```

