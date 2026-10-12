# Studio Prompt Afiliat

App web satu fail (`index.html`) untuk menyusun prompt video afiliat dalam Bahasa Melayu, berdasarkan modul "Dari Prompt Sampai Cuan" (Nayaka Design Creator).

## Cara guna

Buka `index.html` dalam browser. Tiada server atau pemasangan diperlukan.

1. Isi nama produk, rupa produk, latar, warna brand, masalah pembeli dan kelebihan.
2. Pilih kategori: Makanan, Minuman, Gadget, Barang rumah, Fashion, Kasut, Kosmetik atau Skincare.
3. Pilih jenis video:
   - **Iklan 30 saat**: storyboard di ChatGPT, kemudian 3 babak (Hook, Masalah & Penyelesaian, CTA) di Google Flow.
   - **Iklan premium**: kolaj detail produk dan storyboard 6 panel, kemudian 3 klip dengan Set A/B dan satu kod kamera.
   - **5 babak**: 5 gambar (Hook, Detail, Demo, Bukti, CTA) yang dijadikan video dengan prompt gerak.
   - **ASMR**: storyboard ASMR 6 panel, tanpa muzik dan narasi.
4. Salin setiap prompt mengikut langkah ChatGPT, Google Flow dan CapCut, kemudian tulis kapsyen TikTok.

App memilih kod visual sendiri ikut kategori, contohnya `/drink_splash` untuk hook minuman atau `/fashion_catalog` untuk babak bukti fashion. Ayat PRODUCT LOCK ditambah secara automatik supaya logo, label dan bentuk produk tidak berubah.

Tab **Kamus Kod** menyenaraikan 34 kod gambar, tag Google Flow dan kod camera direction. Tab **Bonus** mengandungi prompt tool generator Gemini, animasi Pixar dan claymation.

Data borang disimpan dalam `localStorage` browser anda sahaja.

## Ubah kod pilihan

Semua peraturan ada dalam objek `KAT` (tetapan setiap kategori), `CMD` (34 kod gambar) dan `FLOW` (kombinasi tag Google Flow) di dalam `<script>`.
