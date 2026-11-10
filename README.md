# Akuisisi Data Akomodasi Kecamatan Kintamani

Praktikum mata kuliah **BIFP-243 Akuisisi dan Manajemen Data** menggunakan OpenStreetMap untuk mengumpulkan dan mengolah data akomodasi di Kecamatan Kintamani, Kabupaten Bangli, Bali.

## Identitas Mahasiswa

- **Nama:** I Gusti Lanang Agung Wahyu Pandu Rangga
- **NIM:** 2501010026
- **Mata Kuliah:** BIFP-243 Akuisisi dan Manajemen Data

## Tujuan

Memahami proses pengambilan data menggunakan API, mengolah data mentah menjadi tabel, memeriksa kualitas data, serta menampilkan persebaran akomodasi di Kecamatan Kintamani.

## Sumber Data

1. [OpenStreetMap](https://www.openstreetmap.org/) melalui [Overpass API](https://overpass-api.de/api/interpreter).
2. [BPS Kabupaten Bangli](https://banglikab.bps.go.id/) sebagai sumber data pembanding.

Data OpenStreetMap menggunakan lisensi ODbL.

## Metode Akuisisi

Proses dilakukan melalui tahapan berikut:

1. Mengambil data akomodasi menggunakan Overpass API.
2. Menerapkan retry apabila permintaan API gagal.
3. Menyimpan data mentah dalam format JSON.
4. Mengubah data JSON menjadi tabel menggunakan Pandas.
5. Memeriksa kelengkapan dan kesesuaian data.
6. Melakukan verifikasi sampel.
7. Membuat visualisasi persebaran akomodasi menggunakan Matplotlib.

## Batasan dan Etika

- Menggunakan sumber data terbuka.
- Tidak melakukan scraping dari OTA maupun Google Maps.
- Tidak mengambil data kontak pribadi.
- Mematuhi batas penggunaan API.
- Tetap mencantumkan atribusi OpenStreetMap.

Atribusi: © OpenStreetMap contributors. [Lisensi ODbL](https://www.openstreetmap.org/copyright).

## Cara Menjalankan

Instal library yang diperlukan:

```bash
pip install requests pandas matplotlib jupyter
```

Jalankan Jupyter Notebook:

```bash
jupyter notebook
```

Buka dan jalankan file:

```text
notebooks/akuisisi_akomodasi.ipynb
```

**Catatan:** Menjalankan ulang notebook akan mengambil data baru dari Overpass API, kecuali program menggunakan kembali data mentah yang sudah tersimpan di `data/raw/`.

## Hasil

Hasil praktikum berupa:
- Data akomodasi dalam bentuk tabel.
- Perbandingan dan pemeriksaan kualitas data.
- Verifikasi sampel.
- Grafik persebaran akomodasi Kecamatan Kintamani.