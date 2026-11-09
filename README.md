# Akuisisi Data Akomodasi di Kecamatan Kintamani

Mata kuliah BIFP-243 Akuisisi dan Manajemen Data
Nama / NIM: TODO

## Tujuan
TODO: jelaskan dengan kalimat sendiri.

## Sumber data
- OpenStreetMap melalui Overpass API (https://overpass-api.de/api/interpreter), lisensi ODbL.
- BPS TODO (publikasi, tahun) sebagai pembanding.

Data: (c) OpenStreetMap contributors. Lisensi ODbL: https://www.openstreetmap.org/copyright

## Tanggal akses
TODO (lihat docs/provenance.json)

## Metode akuisisi
TODO: ringkas query, retry, penyimpanan data mentah, perataan tabel.

## Batasan etika
TODO: tidak ada scraping OTA/Google Maps; tidak mengambil data kontak; batas pemakaian dipatuhi.

## Cara menjalankan ulang
```
pip install requests pandas matplotlib jupyter
jupyter nbconvert --to notebook --execute notebooks/akuisisi_akomodasi.ipynb
```
Catatan: menjalankan ulang akan memanggil Overpass lagi kecuali berkas mentah sudah ada di data/raw/.
