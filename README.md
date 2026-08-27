# Laporan UTBK 2027

Presentasi Beamer untuk sosialisasi program pembimbingan UTBK 2027 di SMAN 1 Muntilan bersama StudentPro.

## Kompilasi

Jalankan perintah berikut dari direktori utama repositori:

```bash
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

Hasil kompilasi tersedia sebagai `main.pdf`.

## Struktur modular

- `main.tex`: dokumen utama dan urutan bab.
- `konfigurasi/preamble.tex`: paket, warna, tipografi, footer, dan perintah bersama.
- `bab/*.tex`: konten frame setiap bab tanpa `documentclass` dan tanpa lingkungan `document`.

Untuk menambah bab:

1. Buat file baru di dalam direktori `bab/`.
2. Awali dengan nomor bab, judul, subjudul, dan tanggal.
3. Tambahkan `input` file tersebut pada `main.tex`.
4. Kompilasi ulang `main.tex`.

## Bab yang sudah tersedia

1. Pendahuluan.
2. Struktur dan materi UTBK 2026.
3. Proyeksi UTBK 2027.
4. Pelaksanaan pembimbingan UTBK 2026.
5. Evaluasi program SMAN 1 Muntilan.
6. Peta materi dan kurikulum operasional UTBK.

Informasi resmi UTBK 2026, proyeksi 2027, dan data internal harus selalu diberi status yang jelas serta disertai sumber pada bagian akhir bab.
