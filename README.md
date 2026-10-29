# KAMERA·AI — Deteksi Wajah di Peramban

Aplikasi web satu halaman untuk deteksi wajah secara langsung dari kamera,
foto demo, atau foto unggahan. Seluruh pemrosesan berjalan di perangkat
pengguna (di peramban), tanpa mengirim gambar ke server.

## Fitur

- Perkiraan usia, pria/wanita (dengan persentase keyakinan; di bawah 65%
  ditampilkan sebagai "Belum yakin"), dan emosi dominan lengkap dengan rincian.
- Persentase senyum, mata terbuka (landmark mata), jumlah dan ukuran wajah.
- Panel kondisi: indikator kantuk dari kedipan dan gerakan kepala (mode kamera).
- Panel kulit: skor tampilan kulit dari piksel foto. Bukan diagnosis medis.
- Panel aksesori dan pakaian: warna dominan dan pola, dengan tautan cek
  merek dan harga di Google Shopping.
- Deteksi barang yang mungkin dipegang (80 jenis objek, COCO-SSD) dengan
  tautan cek harga dan gambar serupa.
- Pencocokan visual lewat Google dan Google Lens dari cuplikan hasil.
- Mode gelap dan terang, tampilan ramah HP, bisa dipasang ke layar utama (PWA).

## Catatan Kejujuran

- Kolom negara/region di aplikasi adalah **SIMULASI** (tebakan acak berlabel
  jelas di halaman). Negara seseorang tidak dapat dideteksi dari wajah.

## Teknologi

- face-api.js (model dimuat dari CDN jsDelivr) dan COCO-SSD untuk deteksi objek.
- Kamera membutuhkan koneksi aman (https). GitHub Pages memenuhi syarat ini.

## Menjalankan

Aktifkan GitHub Pages (Settings → Pages → Deploy from a branch → main → / (root)).
Struktur repository harus utuh: `index.html` di root dan folder `assets/` di sebelahnya.
