# Panduan Video Pembelajaran (Google Drive & File Lokal)

Untuk video pembelajaran berkapasitas besar (misal: 100MB - 2GB+, rekaman PPL / UKIN berdurasi panjang 30-90 menit), sangat disarankan menggunakan **Google Drive** agar website tetap ringan dan cepat saat diakses penguji atau umum.

---

## 🚀 Cara Menautkan Video Google Drive (Bisa Dilihat Semua Orang)

### Langkah 1: Upload Video ke Google Drive
1. Buka [Google Drive](https://drive.google.com).
2. Buat folder baru (misal: `Video Pembelajaran PPG`) atau upload langsung video MP4 Anda.

### Langkah 2: Atur Izin Akses Menjadi Publik
Agar video bisa dilihat oleh dosen penguji, penilai UKIN, dan semua orang tanpa perlu meminta izin akses:
1. Klik kanan file video di Google Drive > pilih **Bagikan (Share)** > klik **Bagikan**.
2. Di bagian **Akses umum (General access)**:
   - Ubah dari **"Dibatasi" (Restricted)** menjadi **"Siapa saja yang memiliki link" (Anyone with the link)**.
   - Perannya biarkan sebagai **"Pelihat" (Viewer)**.
3. Klik tombol **"Salin link" (Copy link)** > klik **Selesai**.

### Langkah 3: Tempelkan Link ke `index.html`
1. Buka file `index.html`.
2. Cari bagian `<!-- VIDEO 1: Senam Aerobik -->` atau `<!-- VIDEO 2: Senam Lantai Kelas X -->`.
3. Ganti link placeholder `https://drive.google.com/file/d/.../view?usp=sharing` dengan link yang baru saja Anda salin pada:
   - Atribut `href="..."` pada tombol `<a class="btn-gdrive">`
   - Parameter pertama pada fungsi `openGoogleDriveModal('LINK_GDRIVE_ANDA', 'Judul Video')`

---

## 📁 Opsi Video File Lokal (Cadangan)
Jika video berukuran di bawah 50MB dan ingin dijalankan langsung secara offline di localhost:
- Simpan file video Anda di folder `video-pembelajaran/`.
- Tautan cadangan lokal sudah otomatis tersedia di bawah setiap kartu video.
