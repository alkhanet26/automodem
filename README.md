# AUTO RESTART MODEM untuk OPENWRT ALKHANET

script ini untuk auto reboot modem usb stick/ modem bypass di firmware openwrt mod ALKHANET karena proses nya mutus arus USB
paket pendukung httping

```
opkg update && opkg install httping
```


```
wget --no-check-certificate "https://raw.githubusercontent.com/alkhanet26/automodem/main/automodem" -O /sbin/automodem && chmod +x /sbin/automodem
```

Setelah proses installasi selesai,,, tambahkan perintah di ``schedule task``
```
*/2 * * * * sh /sbin/automodem youtube.com
```
