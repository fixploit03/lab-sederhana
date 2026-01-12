# dnsmasq

`dnsmasq` adalah perangkat lunak open-source ringan yang menyediakan layanan jaringan penting untuk jaringan kecil hingga menengah, terutama sebagai server DNS (Domain Name System) dan DHCP (Dynamic Host Configuration Protocol) yang mudah dikonfigurasi, serta dapat berfungsi sebagai server TFTP dan mendukung Router Advertisement. 

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
