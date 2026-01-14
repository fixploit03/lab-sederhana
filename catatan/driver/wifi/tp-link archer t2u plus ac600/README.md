# TP-LINK Archer T2U Plus AC600

## Cara Instal

#### 1. Update Repositori Kali Linux

```
sudo apt-get update
```

#### 2. Instal Dependensi yang Dibutuhkan

```
sudo apt-get install linux-headers-$(uname -r) build-essential bc dkms git libelf-dev rfkill iw
```

#### 3. Kloning Driver

```
git clone https://github.com/morrownr/8821au-20210708.git
```

#### 4. Pindah ke Direktori Driver

```
cd 8821au-20210708
```

#### 5. Instal Driver

```
sudo ./install-driver.sh
```

#### 6. Verifikasi Driver

```
lsmod | grep 8821au
```
