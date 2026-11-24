# SIM-AKREDITASI S2
Prototipe aplikasi lokal untuk FUPS Magister, Lampiran 34 LAMSPAK 9/2024. Lampiran 5 menjadi referensi evaluasi; instrumen BAN-PT 8/2020 magister terapan hanya pembanding. Belum diverifikasi terhadap regulasi terkini atau asesor.

## Menjalankan
Buka index.html bersama app.js dalam satu folder. Untuk penyimpanan lokal yang lebih konsisten, jalankan `python -m http.server 8000` di folder tersebut dan buka http://localhost:8000.

## GitHub Pages
Buat repository `Instrumen-Minimum-Dokumen-Usulan-Akreditasi-Program-Studi-S2`, unggah isi folder ini ke root branch main. Settings > Pages > Build and deployment > Deploy from a branch > main / (root) > Save. Akses URL yang ditampilkan GitHub setelah deployment.

## Penggunaan
- Muat contoh lengkap: draf hipotetis Magister Administrasi Publik dengan 14 butir; bukti yang belum ada ditandai, bukan direkayasa.
- Reset pengisian: konfirmasi sebelum menghapus data lokal.
- Ekspor Word: DOCX asli, dapat diedit; ekspor PDF: dialog cetak browser, pilih Save as PDF/Simpan sebagai PDF.
- Cadangkan/Impor JSON: simpan/pulihkan isian. Data tersimpan lokal pada browser, bukan GitHub. Jangan unggah cadangan yang mengandung data pribadi.
- Daftar dokumen mencatat status dan lokasi bukti, bukan mengunggah berkas. Pemeriksaan hanya kelengkapan dasar, bukan skor akreditasi.

## Batasan
Format tabel diadaptasi dari sembilan tabel Lampiran 34 (ditambah matriks pendukung); bukan reproduksi persis tata letak resmi. Pakta integritas merupakan draf yang harus dicocokkan dengan redaksi resmi. Tidak ada autentikasi, kolaborasi server, pemeriksaan keaslian berkas atau integrasi PDDikti. Konflik aturan dicatat untuk klarifikasi. Validasi empiris dengan asesor dan data riil belum dilakukan.

## Versi 2.0 — Review dokumen (@ramalabs)
- Pilih menu **Review dokumen**. Unggah PDF berbasis teks, DOCX, atau TXT; atau tempel teks. Periksa hasil ekstraksi, lalu klik Mulai review. Format judul mengikuti nomor 1–14 Lampiran 34; judul yang berbeda atau terpecah dapat tidak terdeteksi. DOCX menggunakan nomor paragraf, PDF nomor halaman.
- Mesin review deterministik mencocokkan istilah dalam bagian yang terdeteksi. Kutipan, kekurangan potensial, rekomendasi, catatan reviewer, dan rujukan halaman tersedia untuk 14 butir. Tidak memeriksa keaslian, kecukupan substantif, angka atau tautan secara otomatis. Tidak menggunakan AI generatif. Tidak memberikan skor resmi. Perbedaan Lampiran 34 dan 5 tetap dicatat. Lampiran BAN-PT 2020 tidak diterapkan untuk magister akademik.
- Ekspor review ke DOCX atau cetak PDF (Save as PDF). Footer @ramalabs. Reset review terpisah dari reset formulir. Review hanya disimpan sementara di memori; ekspor sebelum menutup halaman. Data formulir tetap menggunakan penyimpanan lokal.
- PDF memerlukan koneksi internet untuk pustaka PDF.js 4.10.38 dari jsDelivr; file diproses di browser. DOCX memerlukan browser modern dengan DecompressionStream (deflate-raw). PDF pindai perlu OCR eksternal. Jangan gunakan dokumen sensitif pada perangkat bersama; untuk penggunaan institusional audit dependensi dan keamanan terlebih dahulu.
- Pengujian saat pembuatan: syntax JavaScript dan unit test aturan dasar. Pengujian browser end-to-end serta validasi ahli belum dilakukan. Status regulasi per 2026 belum diverifikasi.
- Unggah seluruh file dalam ZIP (index.html, app.js, review-engine.js, review.js, README.md) ke root repository dan aktifkan GitHub Pages.

## Deployment otomatis (paket GitHub-ready)
Pilihan A: unggah semua file termasuk `.github/workflows/pages.yml` melalui Git atau GitHub Desktop. Buka Settings > Pages > Source > GitHub Actions. Pada tab Actions, pilih Deploy SIM-AKREDITASI S2 > Run workflow jika belum berjalan. URL tersedia pada Settings > Pages setelah deployment sukses.

Pilihan B (unggah melalui browser, tanpa workflow): unggah lima file utama dan `.nojekyll` jika tersedia. Buka Settings > Pages > Deploy from a branch > main > / (root) > Save. Gunakan hanya salah satu metode deployment. Jangan unggah dokumen usulan, KTP, ijazah, atau cadangan JSON.
