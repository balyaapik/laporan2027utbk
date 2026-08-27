# Laporan UTBK 2027

Presentasi Beamer untuk sosialisasi program pembimbingan UTBK 2027 di SMAN 1 Muntilan bersama StudentPro.

## Kompilasi

Jalankan perintah berikut dari direktori utama repositori:

```bash
mkdir -p output/pdf
pdflatex -interaction=nonstopmode -output-directory=output/pdf main.tex
bibtex output/pdf/main
pdflatex -interaction=nonstopmode -output-directory=output/pdf main.tex
pdflatex -interaction=nonstopmode -output-directory=output/pdf main.tex
```

Hasil kompilasi tersedia sebagai `output/pdf/main.pdf`.

## Struktur modular

- `main.tex`: dokumen utama dan urutan bab.
- `konfigurasi/preamble.tex`: paket, warna, tipografi, footer, dan perintah bersama.
- `bab/*.tex`: konten frame setiap bab tanpa `documentclass` dan tanpa lingkungan `document`.

Untuk menambah bab:

1. Buat file baru di dalam direktori `bab/`.
2. Awali dengan nomor bab, judul, subjudul, dan tanggal.
3. Tambahkan `input` file tersebut pada `main.tex`.
4. Letakkan pemanggilan bab baru sebelum `bab/99-daftar-pustaka` agar bibliografi tetap berada di bagian paling akhir.
5. Kompilasi ulang `main.tex` dan bibliografinya.

## Bab yang sudah tersedia

1. Pendahuluan.
2. Struktur dan materi UTBK 2026.
3. Proyeksi UTBK 2027.
4. Pelaksanaan pembimbingan UTBK 2026.
5. Evaluasi program SMAN 1 Muntilan.
6. Peta materi dan kurikulum operasional UTBK.
7. Contoh soal representatif tujuh subtes UTBK beserta pembahasan.
8. Analisis kesenjangan akademik, proses, data, dan pendampingan.

Informasi resmi UTBK 2026, proyeksi 2027, dan data internal harus selalu diberi status yang jelas. Seluruh sumber dihimpun dalam bibliografi pada bagian paling akhir dokumen.
