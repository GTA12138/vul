# [Information]

**Affected product:** Vitogate 300

**Vendor of the product:** Viessmann

**Product page:** https://connectivity.viessmann.com/gb/mp-fp/vitogate/vitogate-300-bn-mb.html

**Affected system version:** 2.1.3.0 and lower

**Firmware download address:** https://connectivity.viessmann.com/gb/mp-fp/vitogate/vitogate-300-bn-mb/release-historie.html

**Reported by:**  Songyuqing ([q14774807663@gmail.com](mailto:pushe4x@gmail.com))

# [Description]

The Vitogate 300, the gateway used to connect the Viessmann LON to BACnet or Modbus, was deployed with a problem that allowed an attacker to access sensitive content such as configuration files without logging in.

# [Vulnerability details]

When we use directory scanning software like dirsearch, we can access and download these scanned directories without any authentication.It's very easy to get the configuration information of the server and the accounts and passwords and other related content

You can find the accounts and passwords stored there. Username: vitomaster, password: viessmann1917

![1](.\1.png)

![2](.\2.jpg)

![3](.\3.jpg)

![4](.\4.png)

![5](.\5.png)
