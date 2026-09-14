# ENV Monitoring Dashboard 2026

Aplikasi dashboard pemantauan lingkungan yang berjalan sepenuhnya di browser.
Tidak ada server, tidak ada basis data, tidak ada pengiriman data ke mana pun.

**Buka di sini:** https://claudesharing2-creator.github.io/projectexcel/

## Isi repositori ini

| Berkas | Keterangan |
|---|---|
| `index.html` | Aplikasinya, sudah jadi |
| `ocr-model.json` | Mesin pembaca teks dari gambar (OCR), diambil hanya saat fitur OCR dipakai |
| `.nojekyll` | Menonaktifkan pemrosesan Jekyll di GitHub Pages |
| `README.md` | Berkas ini |

Seluruh aplikasi ada di dalam `index.html`. Satu-satunya bagian yang dipisah
adalah mesin OCR: ukurannya 9,5 MB dan dulu ikut terunduh setiap kali halaman
dibuka, padahal hanya terpakai kalau pengguna membaca teks dari PDF hasil
pindaian. Sekarang berkas itu baru diambil saat OCR pertama kali dijalankan,
lalu tersimpan di browser sehingga pemakaian berikutnya tidak mengunduh apa pun
lagi — termasuk saat sedang luring.

## Datanya tidak ada di sini

Repositori ini **publik**, jadi tidak memuat data apa pun: tidak ada hasil
sampling, nomor dokumen, koordinat lokasi, maupun nama orang. Yang tampil saat
aplikasi dibuka pertama kali hanyalah nilai contoh.

Data sebenarnya disimpan terpisah dalam berkas **Data Pack** milik pengguna,
dan dimuat sendiri lewat menu **ENV Tools → Data Pack**. Data itu hanya
tersimpan di browser pengguna, tidak pernah dikirim ke repositori ini maupun ke
pihak lain.

Kalau aplikasi dibuka tanpa Data Pack, daftar-daftarnya memang kosong — dan
aplikasi akan menyatakan bahwa datanya **belum dimuat**, bukan menyimpulkan
bahwa tidak ada pekerjaan yang tertunda.

## Catatan

Dashboard ini alat bantu penyusunan dan pemantauan. Angka yang ditampilkannya
mengikuti Data Pack yang dimuat pengguna, dan tidak dengan sendirinya menjadi
bukti kepatuhan.
