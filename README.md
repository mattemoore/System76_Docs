# System76_Docs

## Old fix for wifi dying after resuming from suspend
https://random.blackpacket.net/2017/03/system76-delay-resuming-form-suspend/

## Power Management

Another way to help with Wifi issues is to turn off power management for the hardware. To do so, edit the configuration file with this command:
```sudo gedit /etc/NetworkManager/conf.d/default-wifi-powersave-on.conf```  
And change the file to read (effective upon reboot):

```
[connection]
wifi.powersave = 2
```
