# dnsmasq

`dnsmasq` adalah perangkat lunak open-source ringan untuk jaringan kecil hingga menengah yang menyediakan layanan infrastruktur jaringan seperti
DNS forwarding, DHCP server, dan TFTP dalam satu paket, membuatnya ideal untuk router, firewall, dan perangkat IoT dengan sumber daya terbatas karena konfigurasinya yang mudah dan ukurannya yang kecil.

## Cara Instal

```
sudo apt-get update
sudo apt-get install dnsmasq
```

## Cara Menggunakan

#### 1. Konfigurasi IP Address

```
sudo ip addr flush dev [interface]
sudo ip addr add [ip]/[cidr] dev [interface]
sudo ip link set [interface] up
```

#### 2. Jalankan dnsmasq

```
sudo dnsmasq -C [file_config] -d
```
