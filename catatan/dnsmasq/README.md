# Dnsmasq

Dnsmasq adalah perangkat lunak open-source ringan untuk jaringan kecil hingga menengah yang menyediakan layanan infrastruktur jaringan seperti
DNS forwarding, DHCP server, dan TFTP dalam satu paket, membuatnya ideal untuk router, firewall, dan perangkat IoT dengan sumber daya terbatas karena konfigurasinya yang mudah dan ukurannya yang kecil.

## Cara Instal

```
sudo apt update
sudo apt install dnsmasq
```

## Konfigurasi IP Address

```
sudo ip addr flush dev wlan0
sudo ip addr add 10.10.10.1/24 dev wlan0
sudo ip link set wlan0 up
```

## Cara Menggunakan

```
sudo dnsmasq -C dnsmasq.conf -d
```
