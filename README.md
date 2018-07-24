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

### Terminal Details
Linux Version: 2.6.31--LSDK-9.2.0_U10.5.13-GST-A4
GST-2014-11-18-11:17:54

```shell
# cat /proc/version
```
Linux Version 2.6.31--LSDK-9.2.0_U10.5.13-GST-A4 (astro@astro) (gcc version 4.3.3 (GCC)) #44 Tues Nov 18 11:16:25 CST 2014 mips GNU/Linux

```shell
# cat /proc/meminfo
```
Total Memory 62160 kB

```shell
# cat /proc/cpuinfo
```
System Type: Atheros AR9330 (Hornet)
Processor: 0
CPU Model: MIPS 24Kc v7.4
BogoMIPS: 266.24
Wait Instruction: Yes
Microsecond Timers: Yes
tlb_entries: 16
Extra Interrupt Vector: Yes
Hartware Watchpoint: yes, count: 4, address/irw mask: [0x0000, 0x0e00,0x0040, 0x0118]
ASEs Implemented: mips16
Shadow Register sets: 1
core: 0
VCED exceptions: not available
VCEI exceptions: not available

### Accessing Via Telnet
#### 1) Turn on the Smart Battery by pressing and holding the power button for 5 seconds. Once the blue LED is on you can connect to th e
Once you're connected to the router telnet into the device on port 23:
```shell
# telent -l root:root 192.168.1.2 23
```


#### 2) Change the root password
```shell
#  
```

### File & Folder layout
In /tmp folder:
./br0
./dnsmasq.pid  
./ftp
./secath0

./device
./device/ftp
./device/ftp/SDdisk
./device/ftp/SDdisk/SD
./device/ftp/SDdisk/SDUSB

./lock/

./www/
./www/PVT/client/
./www/PVT/client/client.sh
./www/PVT/server/
./www/PVT/server/server.sh

./www/db
./www/header.sh
./www/smartsync_out.sh
./www/PVT.sh
./www/decodeURL
./www/httpd.sh
./www/airsetting_gen
./www/delaycp.sh
./www/image_check.sh
./www/storage_test.sh
./www/airsetting_get
./www/df_date
./www/mime.types
./www/thumbnail_job
./www/ap_scan.sh
./www/diskmark
./www/mount_device
./www/thumbnail_jpeg
./www/apps_check.sh
./www/dns
./www/mount_log
./www/udhcpd.conf
./www/at
./www/dns_start.sh
./www/netled_set.sh
./www/udhcpd.leases
./www/auto_bridge.sh
./www/engmode.sh
./www/noip2
./www/udhcpd_start.sh
./www/auto_copy.sh
./www/ethled.sh
./www/noipenable.sh
./www/udprcv
./www/auto_poweroff.sh
./www/flashburn
./www/pivotroot
./www/udpsend
./www/auto_sta.sh
./www/fr_post.sh
./www/powerlvl
./www/upgradedelay
./www/fr_pre.sh
./www/ppp
./www/url.sed
./www/cfg_info.sta
./www/ghttpd
./www/repeater
./www/usbaddlog.sh
./www/cfg_log
./www/ghttpd.conf
./www/rndis
./www/ghttpd_i
./www/settings
./www/client
./www/gscale
./www/smartsync_in.sh



./www/bridge/Bridge_enable
./www/bridge/bridge_saved.sta
./www/bridge/eth_udhcpc.sh
./www/bridge/wifi_reset.sh
./www/bridge/Bridge_info
./www/bridge/bridgedn.sh 
./www/bridge/ethoverusb_add.sh
./www/bridge/wpa.sta
./www/bridge/ath_udhcpc.sh 
./www/bridge/bridgeup.sh
./www/bridge/udhcpc.script
./www/bridge/bridge 
./www/bridge/eth_check.sh
./www/bridge/unknow_code.conf

./www/cgi-bin/
./www/cgi-bin/cgiNK        
./www/cgi-bin/gdate        
./www/cgi-bin/gfilemanage  
./www/cgi-bin/gota         
./www/cgi-bin/gsync        
./www/cgi-bin/gwds
./www/cgi-bin/gadmin       
./www/cgi-bin/gdb          
./www/cgi-bin/gfind        
./www/cgi-bin/gpoweroff    
./www/cgi-bin/gthumbnail   
./www/cgi-bin/gwmac
./www/cgi-bin/gantenna     
./www/cgi-bin/gddns        
./www/cgi-bin/gflashburn   
./www/cgi-bin/gproduct     
./www/cgi-bin/gupload      
./www/cgi-bin/gwman
./www/cgi-bin/gbattery     
./www/cgi-bin/gdefault     
./www/cgi-bin/gidle        
./www/cgi-bin/gscandir     
./www/cgi-bin/guser        
./www/cgi-bin/gwmana4
./www/cgi-bin/gbridge      
./www/cgi-bin/gdhcpset     
./www/cgi-bin/ginfo        
./www/cgi-bin/gscsi        
./www/cgi-bin/gusertable   
./www/cgi-bin/id3
./www/cgi-bin/gchannel     
./www/cgi-bin/gdownload    
./www/cgi-bin/glogo        
./www/cgi-bin/gserverip    
./www/cgi-bin/gversion     
./www/cgi-bin/reboot
./www/cgi-bin/gclient      
./www/cgi-bin/getupdate    
./www/cgi-bin/gnetif       
./www/cgi-bin/gstorage     
./www/cgi-bin/gwan         
./www/cgi-bin/tct_ev_proc

./www/client/udhcpc.script

./www/db/dbfunct.sh  
./www/db/dbpoll.sh 
./www/db/dbsync.sh 
./www/db/global

./www/dns/dns_conf.sh
./www/dns/dnsmasq.hosts
./www/dns/dnsmasq.conf
./www/dns/resolv.dnsmasq.conf

./www/ppp/ip-down
./www/ppp/pppoe-start.sh
./www/ppp/add.sh 
./www/ppp/ip-up
./www/ppp/pppoe-stop.sh
./www/ppp/add2.sh 
./www/ppp/ipv6-down
./www/ppp/pppoe.conf
./www/ppp/apn_check.sh 
./www/ppp/ipv6-up 
./www/ppp/pppoe_on_boot
./www/ppp/apns.xml 
./www/ppp/modem 
./www/ppp/provider
./www/ppp/chap-secrets 
./www/ppp/modem-connect-chat
./www/ppp/removea4.sh
./www/ppp/chat3g.template
./www/ppp/options.pptp
./www/ppp/resolv.conf
./www/ppp/options.wman 
./www/ppp/rssi_get.sh
./www/ppp/display_enable.sh
./www/ppp/pap-secrets
./www/ppp/turnon3g
./www/ppp/display_sleep.sh
./www/ppp/ppp_set.sh 
./www/ppp/wman_enable.sh
./www/ppp/gprs-connect-chat
./www/ppp/pppoe-connect.sh 
./www/ppp/wman_power.sh
./www/ppp/device/

./www/repeater/rootap_set.sh

./www/rndis/add.sh
./www/rndis/udhcpc.script

./www/settings/index.html

./www/settings/bootstrap/css
./www/settings/bootstrap/css/bootstrap-responsive.min.css
./www/settings/bootstrap/css/bootstrapSwitch.css
./www/settings/bootstrap/css/bootstrap.min.css

./www/settings/bootstrap/img
./www/settings/bootstrap/img/glyphicons-halflings-white.png
./www/settings/bootstrap/img/glyphicons-halflings.png

./www/settings/bootstrap/js
./www/settings/bootstrap/js/bootbox.min.js
./www/settings/bootstrap/js/bootstrap.min.js

./www/settings/css/style.css

./www/settings/images/ajax-loader-1.gif
./www/settings/images/anim_wait_bar_mini_01.gif
./www/settings/images/ajax-loader-2.gif
./www/settings/images/logo-nimble-apps.png

./www/settings/img/ajax-loader.gif
./www/settings/img/lock_strength3.png
./www/settings/img/glyphicons-halflings-white.png
./www/settings/img/online.png
./www/settings/img/glyphicons-halflings.png
./www/settings/img/strength0.png
./www/settings/img/lock_strength0.png  
./www/settings/img/strength1.png
./www/settings/img/lock_strength1.png
./www/settings/img/strength2.png
./www/settings/img/lock_strength2.png
./www/settings/img/strength3.png

./www/settings/js/bootstrapSwitch.js
./www/settings/js/jquery.form.min.js
./www/settings/js/jquery.validate.js
./www/settings/js/jquery-1.9.0.min.js
./www/settings/js/jquery.localize.min.js
./www/settings/js/jquery.cookie.js 
./www/settings/js/jquery.nimble.loader.js

./www/settings/js/lang/
./www/settings/js/lang/example-en.json
./www/settings/js/lang/example-tw.json

./www/storage/
./www/storage/a6usbreset.sh
./www/storage/check_filesystem_type
./www/storage/remove.sh
./www/storage/add.sh
./www/storage/df_check.sh
./www/storage/auto_a6usbreset.sh
./www/storage/reflash.sh

