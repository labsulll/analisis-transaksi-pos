# Analisis Pendapatan Transaksi POS Tahun 2024–2025

## 1. Deskripsi Project

Project ini merupakan analisis data transaksi Point of Sale (POS) menggunakan Python dan Jupyter Notebook. Analisis dilakukan untuk mengetahui dan membandingkan total pendapatan pada tahun 2024 dan 2025 dengan mempertimbangkan diskon serta status transaksi.

## 2. Tujuan

- Membersihkan dataset dari data kosong, duplikat, dan anomali.
- Mengolah data transaksi menggunakan Python.
- Menghitung pendapatan tahun 2024 dan 2025.
- Membandingkan pendapatan kedua tahun tersebut.
- Menampilkan hasil analisis dalam bentuk visualisasi.

## 3. Tools dan Library

- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn

## 4. Dataset

Dataset yang digunakan adalah data transaksi POS tahun 2024–2025 dengan atribut seperti tanggal transaksi, harga satuan, jumlah barang, diskon, dan status transaksi.

## 5. Tahapan Pengolahan Data

1. Membaca dataset menggunakan Pandas.
2. Memeriksa dan menangani missing values.
3. Menghapus data duplikat.
4. Mengubah format tanggal dan harga agar dapat diolah.
5. Menghapus 52 data anomali, terdiri dari 40 transaksi dengan jumlah negatif dan 12 transaksi dengan jumlah di atas 100.
6. Menghitung pendapatan dengan mempertimbangkan diskon dan status transaksi.

## 6. Metode Perhitungan Pendapatan

Pendapatan dihitung menggunakan rumus:

**Pendapatan = Jumlah × Harga Satuan × (1 − Diskon/100)**

Perlakuan status transaksi:
- **SELESAI:** Pendapatan dihitung setelah diskon.
- **BATAL:** Tidak dihitung sebagai pendapatan.
- **RETUR:** Dikurangkan dari total pendapatan.

## 7. Hasil Analisis

Jumlah data setelah proses pembersihan adalah **4.948 baris**.

| Keterangan | Hasil |
|---|---:|
| Pendapatan 2024 | Rp125.119.700 |
| Pendapatan 2025 | Rp132.117.975 |
| Selisih pendapatan | Rp6.998.275 |
| Pertumbuhan | 5,59% |

## 8. Kesimpulan

Berdasarkan hasil analisis, pendapatan transaksi POS pada tahun 2025 mengalami peningkatan sebesar 5,59% dibandingkan tahun 2024. Perhitungan telah mempertimbangkan diskon serta status transaksi setelah proses pembersihan data.

## 9. Struktur Project

```text
analisis-transaksi-pos/
├── dataset/
│   └── paket_a_transaksi_pos_2024_2025.csv
├── Analisis_Transaksi_POS.ipynb
├── data_transaksi_bersih.csv
└── README.md
```
