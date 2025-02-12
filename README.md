# laporan-penginstalan-ulinux-ubuntu

# Laporan Penginstalan Linux dengan Gambar

## 1. Persiapan
- Download ISO Linux (contoh: Ubuntu 22.04 LTS) dari [situs resmi Ubuntu](https://ubuntu.com/download).
- Buat bootable USB menggunakan *Rufus* atau *Balena Etcher*.
- Pastikan perangkat memiliki minimal:
  - RAM 4 GB
  - Penyimpanan 20 GB

---

## 2. Langkah-langkah Instalasi

### *Langkah 1: Boot dari USB*
- Colokkan USB Bootable dan nyalakan komputer.
- Tekan *F12* atau *ESC* untuk masuk ke Boot Menu.
- Pilih *USB Drive* sebagai media booting.  
- Tampilan awal seperti di bawah ini:

![Langkah 1 - Boot](images/langkah-1-boot.png)

---

### *Langkah 2: Welcome Screen*
- Pilih bahasa yang diinginkan.
- Klik *Install Ubuntu* untuk melanjutkan.  

![Langkah 2 - Welcome](images/langkah-2-welcome.png)

---

### *Langkah 3: Setting Partisi*
- Pilih opsi *Something else* untuk partisi manual.
- Atur partisi sebagai berikut:
  - Root (/) minimal 20 GB
  - Swap sesuai kapasitas RAM
  - Home (/home) untuk penyimpanan data pengguna  

![Langkah 3 - Partisi](images/langkah-3-partisi.png)

---

### *Langkah 4: Proses Instalasi*
- Masukkan detail pengguna:
  - Nama pengguna
  - Username
  - Password
- Klik *Install Now* dan tunggu hingga selesai.  

![Langkah 4 - Instalasi](images/langkah-4-instalasi.png)

---

## 3. Konfigurasi Pasca Instalasi
- Update sistem menggunakan perintah:
    bash
    sudo apt update && sudo apt upgrade -y
    
- Instal aplikasi tambahan:
    bash
    sudo apt install vim git curl
    

---

## 4. Troubleshooting
- Jika mengalami masalah booting:
  - Periksa *Boot Order* di BIOS/UEFI.
  - Gunakan *Boot Repair* dari live USB.

---

## 5. Kesimpulan
Proses instalasi berjalan lancar dan sistem siap digunakan untuk kebutuhan pengembangan dan produktivitas sehari-hari.
