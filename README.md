# Gigastone-Smart-Battery-A4-52ER
Tweaking and Re-leveraging the Gigastone Smart Battery A4-52ER via Telnet. This portable battery can sometimes be found for $15 from some sellers as of 2018. 

### Specifications
Li-Ion Batter: 5200mAh
Charge In: DC 5V/1000mA
Charge Out: DC 5V/1000mA
SD Card: SDHC, SDXC
USB Drive: 2.0 & 3.0
Wireless I/F: WiFi 802.11 b/g/n
WiFi Operation Time: Up to 16 Hrs
Operation Temp: 0C ~ 40C / 32F ~ 104F

### Operating Instructions
Power: Press on/off button for 5 seconds and blue LED light will light up or turn off.
Check Battery Life: Press on/off button, green LED lights indicated battery level and connected devices recieve power.
Access Smart Box via Browser: 192.168.1.2 in the browser.
Default Admin (Device Web Admin Portal) Password: 0000 

### Accessing Via Telnet
1) Turn on the Smart Battery by pressing and holding the power button for 5 seconds. Once the blue LED is on you can connect to th e
Once you're connected to the router telnet into the device on port 23:
```shell
$ telent -l root:root 192.168.1.2 23
```


### File layout
