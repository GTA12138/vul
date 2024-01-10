**Affected product:**Byzro Networks Smart S150 management platform

**Vendor of the product:** Byzro Networks Smart S150 management platform

**Product page:** https://connectivity.viessmann.com/gb/mp-fp/vitogate/vitogate-300-bn-mb.html

**Affected system version:** S150

**Firmware download address:** 

https://218.205.129.204:8443/patrolflow.php


**Reported by:** Songyuqing ([q14774807663@gmail.com](mailto:pushe4x@gmail.com))

# [Description]

Where backup files are configured, there is no filtering of parameters for downloading files, which can result in the downloading of arbitrary sensitive files such as passwd

# [Vulnerability details]

Where backup files are configured, there is no filtering of parameters for downloading files, which can result in the downloading of arbitrary sensitive files such as passwd



First login to our example server, click Device Management - Configuration Management - Download Backup File(设备管理-配置管理-下载备份文件), and then use burpsuite to capture the packet, we can see the filename, when we change the filename parameter to, passwd, we find that the device still executes our request and downloads the passwd file

and you can use this url to test:https://218.205.129.204:8443/log/download.php?local=yes&type=filedown&file=L2V0Yy9wYXNzd2Q=&filename=passwd



Proof of network-wide assets, with over 1000 ip's using the system

![](https://github.com/GTA12138/vul/blob/main/smart%20s150/6.png)



admin/b3f9t8k7

![](https://github.com/GTA12138/vul/blob/main/smart%20s150/5.png)



![](https://github.com/GTA12138/vul/blob/main/smart%20s150/s150%20Download%20any%20file/a.png)

![](https://github.com/GTA12138/vul/blob/main/smart%20s150/s150%20Download%20any%20file/b.png)

![](https://github.com/GTA12138/vul/blob/main/smart%20s150/s150%20Download%20any%20file/c.png)

![](https://github.com/GTA12138/vul/blob/main/smart%20s150/s150%20Download%20any%20file/e.png)

![](https://github.com/GTA12138/vul/blob/main/smart%20s150/s150%20Download%20any%20file/d.png)
