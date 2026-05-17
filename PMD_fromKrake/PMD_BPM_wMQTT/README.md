## Summary
An ESP32 project.
Based on an ESP32 Dev Kit1
As of about Jun 15 2025, Device connects to a WiFi network with WiFi Manager and device accept OTA update with Eligant OTA.

## Future features
Incrementally add the following features.

1. Increment the version
2. Serve a web page which identifies the device as FILE_NAME (PMD_BPM_MQTT) and version number. The home web page will have a link to the update page.
3. The OLED display will report the status of the Wi-Fi initialization. It will show the Wi-Fi type such as soft AP or STA. It will report the device MAC address.
It will report the IP address of the Soft AP or the STA.  This splash screen will stay visible for five seconds. After which the progream resumes as per its current behavior. There is a active low button on GPIO35. Pressing it for a time greater than a debounce time and less than 1 second will cause the splash screen to again display, again for 5 seconds.
4. [x] During boot, after the stage reporting "Loaded WiFi credentials from storage." Display on OLED and print to Serial Monitor the credentials so that a user could know and trouble shoot WiFi connection problems.
5. Change the default MQTT broker from "public.cloud.shiftr.io" to "krakepubinv.cloud.shiftr.io". Make so can choose one or other using an ifdef where the compile defin is "PUBLIC_BROKER" for "public.cloud.shiftr.io". So if not "PUBLIC_BROKER" then "krakepubinv.cloud.shiftr.io". Increment the version.
6. TBD...


## Boot message as of V.0.1.11
```
ets Jul 29 2019 12:21:46

rst:0x1 (POWERON_RESET),boot:0x13 (SPI_FAST_FLASH_BOOT)
configsip: 0, SPIWP:0xee
clk_drv:0x00,q_drv:0x00,d_drv:0x00,cs0_drv:0x00,hd_drv:0x00,wp_drv:0x00
mode:DIO, clock div:1
load:0x3fff0030,len:1344
load:0x40078000,len:13924
ho 0 tail 12 room 4
load:0x40080400,len:3600
entry 0x400805f0
E (345) ADC: adc1_lock_release(419): adc1 lock release called before acquire
===================================
PMD_BPM_wMQTT  V.0.1.11
Model: HW2_WiFiReady_Elegant
SN: 00001
Compiled at: May 16 2026 07:31:32
GNU Affero General Public License, version 3
===================================

LittleFS mounted successfully.
Loaded WiFi credentials from storage.
WiFi credentials loaded from LittleFS:
  SSID: <stored-ssid>
  Password: <stored-password>
Connected to WiFi!
Connecting to WiFi ....

```

