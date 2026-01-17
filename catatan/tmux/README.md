# Tmux

Tmux (Terminal Multiplexer) adalah tool di Linux/Unix yang memungkinkan kamu menjalankan banyak sesi terminal dalam satu layar, membaginya menjadi beberapa panel, jendela, dan sesi, serta tetap berjalan walaupun koneksi SSH terputus.

## Cara Instal

```
sudo apt-get update
sudo apt-get install tmux
```

## Cara Menggunakan

#### Membuat Sesi Baru

```
tmux
```

Atau dengan nama sesi tertentu:

```
tmux new -s [nama_sesi]
```

#### Detach (Keluar Tanpa Menutup Proses)

```
Ctrl + b lalu d
```

Sesi tetap berjalan di background.

#### Melihat Daftar Sesi

```
tmux ls
```

#### Masuk Kembali ke Sesi

```
tmux attach -t [nama_sesi]
```

## Shortcut Dasar Tmux

> **Prefix key Tmux =** `Ctrl + b`

#### Jendela

Buat jendela baru:

```
Ctrl + b lalu c
```

Pindah jendela:

```
Ctrl + b lalu n (selanjutnya)
Ctrl + b lalu p (sebelumnya)
```

List jendela:

```
Ctrl + b lalu w
```

#### Split Panel

Split vertikal:

```
Ctrl + b lalu %
```

Split horizontal:

```
Ctrl + b lalu "
```

Pindah panel:

```
Ctrl + b lalu panah ↑ ↓ ← →
```

#### Menutup Panel/Jendela/Sesi

Tutup panel atau jendela yang aktif:

```
exit
```

Tutup satu sesi tertentu:

```
tmux kill-session -t [nama_sesi]
```

Tutup semua sesi:

```
tmux kill-server
```
