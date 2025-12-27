# ASB Network - WiFi Hotspot Template (Bakan Loa)

Template halaman login MikroTik Hotspot yang simpel, responsif, dan modern untuk **ASB Network**. Didesain khusus untuk kemudahan penggunaan pelanggan dengan fitur Trial terintegrasi.

## 🚀 Fitur Utama
* **Desain All-in-One**: CSS dan JavaScript digabung dalam file HTML untuk loading super cepat.
* **Fitur Trial**: Tombol "Coba Gratis 5 Menit" yang muncul otomatis jika fitur Trial aktif di MikroTik.
* **Status Real-time**: Halaman status yang melakukan refresh otomatis setiap 60 detik untuk memperbarui sisa waktu/kuota.
* **Mobile Friendly**: Tampilan optimal di berbagai ukuran layar smartphone.
* **Informasi Bisnis**: Terintegrasi dengan info paket internet rumah dan tombol WhatsApp Admin.

## 📁 Struktur File
Hanya dibutuhkan 3 file utama di dalam folder `hotspot` MikroTik:
1.  `login.html` - Halaman utama untuk memasukkan kode voucher atau mencoba trial.
2.  `status.html` - Halaman informasi sisa waktu dan kuota setelah login.
3.  `logout.html` - Halaman konfirmasi setelah pengguna memutuskan koneksi.

## 🛠️ Panduan Pemasangan

### 1. Persiapan File
* Unggah ketiga file tersebut ke folder `hotspot` melalui **Winbox (Files)** atau **FTP**.

### 2. Pengaturan Walled Garden (Penting!)
Agar font Google (Poppins) muncul dengan benar sebelum user login, tambahkan domain berikut di MikroTik:
* Buka **IP** > **Hotspot** > **Walled Garden**.
* Tambahkan `allow` untuk: `fonts.googleapis.com` dan `fonts.gstatic.com`.

### 3. Mengaktifkan Fitur Trial (5 Menit)
Jika ingin mengaktifkan tombol "Coba Gratis":
1.  Buka **IP** > **Hotspot** > **Server Profiles**.
2.  Pilih profil yang Anda gunakan (contoh: `hsprof1`).
3.  Klik tab **Login**.
4.  Centang **Trial**.
5.  Set **Trial Uptime Limit**: `00:05:00` (5 Menit).
6.  Set **Trial Uptime Reset**: `01:00:00` (User bisa trial lagi setelah 1 hari).

## 📞 Kontak & Dukungan
* **Lokasi**: Wifi Bakan Loa
* **WhatsApp**: 0857 8278 1843
* **Produk**: Voucher WiFi & Internet Unlimited Rumahan

---
*Dibuat untuk ASB Network - Koneksi Cepat & Stabil.*
