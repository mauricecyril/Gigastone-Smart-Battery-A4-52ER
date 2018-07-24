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
Trying 192.168.1.2...
Connected to 192.168.1.2.
Escape character is '^]'.

(none) login: root
Password:
~ # ls
br0          dnsmasq.pid  lock         www
device       ftp          secath0
~ # ls -R
.:
br0          dnsmasq.pid  lock         www
device       ftp          secath0

./device:

./ftp:
SDdisk

./ftp/SDdisk:
SD   USB

./ftp/SDdisk/SD:

./ftp/SDdisk/USB:

./lock:

./www:
PVT               db                header.sh         smartsync_out.sh
PVT.sh            decodeURL         httpd.sh          storage
airsetting_gen    delaycp.sh        image_check.sh    storage_test.sh
airsetting_get    df_date           mime.types        thumbnail_job
ap_scan.sh        diskmark          mount_device      thumbnail_jpeg
apps_check.sh     dns               mount_log         udhcpd.conf
at                dns_start.sh      netled_set.sh     udhcpd.leases
auto_bridge.sh    engmode.sh        noip2             udhcpd_start.sh
auto_copy.sh      ethled.sh         noipenable.sh     udprcv
auto_poweroff.sh  flashburn         pivotroot         udpsend
auto_sta.sh       fr_post.sh        powerlvl          upgradedelay
bridge            fr_pre.sh         ppp               url.sed
cfg_info.sta      ghttpd            repeater          usbaddlog.sh
cfg_log           ghttpd.conf       rndis
cgi-bin           ghttpd_i          settings
client            gscale            smartsync_in.sh

./www/PVT:
client  server

./www/PVT/client:
client.sh

./www/PVT/server:
server.sh

./www/bridge:
Bridge_enable      bridge_saved.sta   eth_udhcpc.sh      wifi_reset.sh
Bridge_info        bridgedn.sh        ethoverusb_add.sh  wpa.sta
ath_udhcpc.sh      bridgeup.sh        udhcpc.script
bridge             eth_check.sh       unknow_code.conf

./www/cgi-bin:
cgiNK        gdate        gfilemanage  gota         gsync        gwds
gadmin       gdb          gfind        gpoweroff    gthumbnail   gwmac
gantenna     gddns        gflashburn   gproduct     gupload      gwman
gbattery     gdefault     gidle        gscandir     guser        gwmana4
gbridge      gdhcpset     ginfo        gscsi        gusertable   id3
gchannel     gdownload    glogo        gserverip    gversion     reboot
gclient      getupdate    gnetif       gstorage     gwan         tct_ev_proc

./www/client:
udhcpc.script

./www/db:
dbfunct.sh  dbpoll.sh   dbsync.sh   global

./www/dns:
dns_conf.sh          dnsmasq.hosts
dnsmasq.conf         resolv.dnsmasq.conf

./www/ppp:
0e8d:0002           ip-down             pppoe-start.sh
add.sh              ip-up               pppoe-stop.sh
add2.sh             ipv6-down           pppoe.conf
apn_check.sh        ipv6-up             pppoe_on_boot
apns.xml            modem               provider
chap-secrets        modem-connect-chat  removea4.sh
chat3g.template     options.pptp        resolv.conf
device              options.wman        rssi_get.sh
display_enable.sh   pap-secrets         turnon3g
display_sleep.sh    ppp_set.sh          wman_enable.sh
gprs-connect-chat   pppoe-connect.sh    wman_power.sh

./www/ppp/device:
0408:1000  12d1:1414  12d1:14c4  12d1:1526  12d1:15e7  12d1:1f11  12d1:1f1e0af0:6971  12d1:1446  12d1:14c5  12d1:1553  12d1:1805  12d1:1f15  19d2:200012d1:1001  12d1:1449  12d1:14d1  12d1:1557  12d1:1c0b  12d1:1f16  1ab7:570012d1:1003  12d1:14ad  12d1:14fe  12d1:155b  12d1:1c1b  12d1:1f17  2001:00a612d1:1009  12d1:14b5  12d1:1505  12d1:156a  12d1:1c24  12d1:1f18  2001:a70712d1:101e  12d1:14b7  12d1:151a  12d1:157c  12d1:1d50  12d1:1f19  feed:567812d1:1030  12d1:14ba  12d1:1520  12d1:157d  12d1:1da1  12d1:1f1b
12d1:1031  12d1:14c1  12d1:1521  12d1:1583  12d1:1f01  12d1:1f1c
12d1:1413  12d1:14c3  12d1:1523  12d1:15ca  12d1:1f03  12d1:1f1d

./www/repeater:
rootap_set.sh

./www/rndis:
add.sh         udhcpc.script

./www/settings:
bootstrap   css         images      img         index.html  js

./www/settings/bootstrap:
css  img  js

./www/settings/bootstrap/css:
bootstrap-responsive.min.css  bootstrapSwitch.css
bootstrap.min.css

./www/settings/bootstrap/img:
glyphicons-halflings-white.png  glyphicons-halflings.png

./www/settings/bootstrap/js:
bootbox.min.js    bootstrap.min.js

./www/settings/css:
style.css

./www/settings/images:
ajax-loader-1.gif          anim_wait_bar_mini_01.gif
ajax-loader-2.gif          logo-nimble-apps.png

./www/settings/img:
ajax-loader.gif                 lock_strength3.png
glyphicons-halflings-white.png  online.png
glyphicons-halflings.png        strength0.png
lock_strength0.png              strength1.png
lock_strength1.png              strength2.png
lock_strength2.png              strength3.png

./www/settings/js:
bootstrapSwitch.js       jquery.form.min.js       jquery.validate.js
jquery-1.9.0.min.js      jquery.localize.min.js   lang
jquery.cookie.js         jquery.nimble.loader.js

./www/settings/js/lang:
example-en.json  example-tw.json

./www/storage:
a6usbreset.sh          check_filesystem_type  remove.sh
add.sh                 df_check.sh
auto_a6usbreset.sh     reflash.sh
~ #
