# SHARIAGUARD

SHARIAGUARD membantu memeriksa isi akad, menandai bagian yang perlu diperhatikan, meminta keputusan DPS, lalu menyimpan riwayat hasil pemeriksaan.

## Fitur

1. **Beranda** — melihat ringkasan alur dan status pemeriksaan.
2. **Simulasi** — menjalankan dua skenario presentasi: alur berhasil dan kasus yang ditolak DPS.
3. **Periksa Akad** — masukkan teks akad dan jalankan pemeriksaan berbasis aturan lokal.
4. **Pemeriksaan DPS** — DPS dapat menyetujui atau menolak setiap bagian yang ditandai.
5. **Catatan Akad** — akad yang lolos pemeriksaan dapat diberi sidik digital SHA-256 dan disimpan.
6. **Riwayat** — melihat aktivitas, pelaku, tindakan, akad, ID catatan, dan sidik.
7. **Referensi** — melihat referensi yang digunakan dalam pemeriksaan.
8. **Akad Baru** — membuat akad baru dengan jenis akad dan pemilik/nasabah contoh.

## Alur utama

**Beranda → Simulasi / Periksa Akad → Pemeriksaan DPS → Catatan Akad → Riwayat**

### Skenario utama

Mudharabah dengan nisbah yang jelas dan satu klausul biaya keterlambatan yang menjadi pendapatan platform.

**Periksa → Temuan → Setujui oleh DPS → Buat sidik digital → Simpan → Lihat Riwayat**

### Kasus masalah

Murabahah tanpa penjelasan harga pokok.

**Periksa → Temuan → Tolak oleh DPS → Pencatatan diblokir → Periksa ulang / Lihat Riwayat**

## Pemeriksaan

Pemeriksaan saat ini adalah prototipe berbasis aturan lokal di browser. Sistem mencari pola tertentu pada teks akad, memberikan nilai pemeriksaan, dan menghasilkan temuan yang perlu ditinjau.

Temuan bukan keputusan hukum Syariah. Keputusan akhir tetap berada pada DPS.

## Data dan privasi

Versi saat ini menyimpan data di localStorage browser pada perangkat pengguna. Data aplikasi tidak dikirim ke server oleh prototype ini.

## Kompatibilitas data

Versi terbaru menggunakan penyimpanan shariaguard-prototype-v5 dan dapat membaca data dari format penyimpanan versi sebelumnya.

## Cara menjalankan

Buka index.html di browser modern, atau gunakan server statis sederhana.

## Deployment

Repository menggunakan GitHub Actions untuk validasi JavaScript dan deployment ke GitHub Pages.

Website: https://xygritte.github.io/SHARIAGUARD/