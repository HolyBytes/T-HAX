# 📱 Panduan Super Gampang Pakai T-HAX Advanced Tool Installer

## ⚠️ PERINGATAN DULU YA, GAES!
* **Tools ini CUMA buat belajar dan pentesting legal aja ya!** Jangan aneh-aneh 🚫
* Beberapa tools perlu **akses root** (`sudo`), jadi siap-siap aja
* Pastiin HP/komputer kamu udah ada **Git, Python, sama PIP** sebelum mulai

## 🔗 Info Penting
* **GitHub**: [https://github.com/HolyBytes/T-HAX.git](https://github.com/HolyBytes/T-HAX.git)
* **Script**: `T-HAX/t-hax.id`
* **Pembuat**: Ade12
* **Lisensi**: © 2023 - All Rights Reserved

## 📋 Daftar Tools Kece yang Bisa Dipasang

| No | Nama Tool | Ukuran | Buat Apa? |
|----|-----------|--------|-----------|
| 1 | Seeker | 10 MB | Ngelacak GPS lewat link phishing |
| 2 | ngrok | 15 MB | Bikin localhost kebuka di internet |
| 3 | Metasploit | 1.5 GB | Framework exploitasi lengkap |
| 4 | Hydra | 5 MB | Nge-crack password |
| 5 | ... | ... | ... |
| 19 | Evil-Droid | 50 MB | Bikin APK jahat buat testing |
| 20 | Routersploit | 30 MB | Exploit router-router |
| 21 | Bettercap | 20 MB | Framework serangan MITM |
| 22 | Netdiscover | 2 MB | Scanner jaringan ARP |

## 🚀 Cara Pasang T-HAX (Step by Step)

### 1️⃣ Persiapan Dulu, Bro/Sis!

**Update dulu Termux/Linux kamu:**
```bash
pkg update && pkg upgrade -y
```
*Kalau pake Linux, ketik aja `sudo apt update && sudo apt upgrade -y` atau `sudo pacman -Syu` tergantung Linux kamu apa*

**Pasang Git biar bisa download:**
```bash
pkg install git -y
```
*Terus cek udah bener belum:*
```bash
git --version
```

**Pasang Python & PIP:**
```bash
pkg install python -y
```
*Cek juga ya:*
```bash
python --version
pip --version
```

**Pasang tools pendukung:**
```bash
pkg install wget curl unzip -y
```

### 2️⃣ Download & Jalanin T-HAX

**Ambil scriptnya dari GitHub:**
```bash
git clone https://github.com/HolyBytes/T-HAX.git
cd T-HAX
```

**Kasih izin buat dijalanin:**
```bash
chmod +x t-hax.id
```

**Gas jalanin:**
```bash
./t-hax.id
```
*Kalau butuh root di Linux, pake `sudo ./t-hax.id`*

## 🛠️ Kalau Ada Error, Jangan Panik!

### ❌ Muncul "Missing Dependencies"?
Beberapa tools butuh paket tambahan.

Misalnya buat Metasploit:
```bash
pkg install ruby -y
gem install bundler
```

Kalau pip ngambek soal setuptools:
```bash
pip install --upgrade setuptools
```

### ❌ Error "No Internet Connection"?
Cek koneksi dulu:
```bash
ping google.com
```
*Kalau perintah `ping` gak ada:*
```bash
pkg install inetutils -y
```

### ❌ Error "Storage Full"?
Beberapa tools (kayak Metasploit) makan banyak tempat.

Bersihin cache:
```bash
pkg clean
```

Cek storage:
```bash
df -h
```

### ❌ Error "Permission Denied"?
Kalau scriptnya gak mau jalan:

Pastiin udah ngasih izin:
```bash
chmod +x t-hax.id
```

Masih gak bisa? Coba:
```bash
bash t-hax.id
```

## 💡 Tips Jitu!

**Kalau download lelet, ganti mirror Termux:**
```bash
termux-change-repo
```
(Pilih mirror kayak `Grimler` atau `BFSU`)

**HP gak di-root? Pake Proot Distro aja:**
```bash
pkg install proot-distro -y
proot-distro install ubuntu
proot-distro login ubuntu
```
(Terus jalanin script di Ubuntu)

**Mau liat log installasi?**
```bash
cat installer.log
```

## 🎉 Akhir Kata

T-HAX dibuat supaya kamu bisa install tools hacking dengan cepat dan gampang. **INGET YA, pake buat belajar aja, jangan iseng sama orang lain!**

**🚀 Selamat Mencoba dan Happy Hacking!**
