# Analisis Sentimen dan Tren Topik Berita Online Indonesia

## Deskripsi Proyek

Proyek akademik kelompok ini membahas penerapan Big Data Analytics untuk mengolah dan menganalisis berita online Indonesia. Proses analisis meliputi penggabungan dataset dari beberapa sumber, pembersihan data, klasifikasi sentimen, pengelompokan topik berita, serta visualisasi hasil analisis.

Analisis sentimen menggunakan model bahasa Indonesia pralatih, sedangkan pengelompokan topik dilakukan menggunakan metode TF-IDF dan algoritma K-Means Clustering.

## Tujuan Proyek

- Menggabungkan dan membersihkan dataset berita dari berbagai sumber.
- Mengidentifikasi distribusi sentimen positif, negatif, dan netral pada berita.
- Mengeksplorasi kelompok topik berita berdasarkan kemiripan teks.
- Memvisualisasikan distribusi sentimen dan topik untuk mempermudah interpretasi data.

## Teknologi yang Digunakan

- **Bahasa pemrograman:** Python
- **Pengolahan data:** Pandas
- **Natural Language Processing (NLP):** Hugging Face Transformers
- **Analisis sentimen:** `w11wo/indonesian-roberta-base-sentiment-classifier`
- **Ekstraksi fitur teks:** TF-IDF
- **Clustering:** K-Means dari Scikit-learn
- **Visualisasi data:** Matplotlib dan Seaborn
- **Lingkungan pengembangan:** Google Colab

## Tahapan Analisis

### 1. Pengumpulan dan Penggabungan Data
Menggabungkan dataset berita dari Kompas, Detik.com, Liputan6, dan dataset berita Indonesia dari Kaggle. Struktur kolom disesuaikan agar data dapat diproses dalam satu dataset.

### 2. Data Cleaning dan Preprocessing
Melakukan pembersihan teks, menghapus data duplikat berdasarkan judul, menangani nilai kosong, serta menyesuaikan format tanggal dan kolom data yang digunakan dalam analisis.

### 3. Analisis Sentimen
Menggunakan model klasifikasi sentimen bahasa Indonesia pralatih untuk mengelompokkan berita ke dalam kategori positif, negatif, dan netral.

### 4. Ekstraksi Fitur dan Clustering
Mengubah teks menjadi representasi numerik menggunakan TF-IDF, kemudian menerapkan K-Means Clustering untuk mengeksplorasi kemiripan dan pengelompokan topik berita.

### 5. Eksplorasi dan Visualisasi Data
Menyajikan hasil analisis melalui bar chart, pie chart, heatmap, stacked bar chart, dan visualisasi distribusi sentimen serta topik berita.

## Hasil Analisis

Berdasarkan laporan proyek kelompok, dataset akhir terdiri dari **67.263 baris berita** dengan distribusi sentimen sebagai berikut:

- **Netral:** 48.991 berita (72,8%)
- **Negatif:** 10.876 berita (16,2%)
- **Positif:** 7.396 berita (11,0%)

Pengelompokan menggunakan K-Means menghasilkan tiga kelompok topik yang dalam proyek diinterpretasikan sebagai Politik, Kriminal, dan Nasional.

> Catatan: hasil clustering merupakan pengelompokan berdasarkan kemiripan teks. Penamaan topik merupakan interpretasi terhadap kelompok yang dihasilkan, bukan label topik yang otomatis diketahui oleh algoritma.

## Dataset

Sumber dataset yang digunakan dalam proyek meliputi:

- Berita dari Kompas, Detik.com, dan Liputan6.
- [Indonesia News Dataset 2024 — Kaggle](https://www.kaggle.com/datasets/sh1zuka/indonesia-news-dataset-2024)

File dataset tidak disertakan dalam repositori ini. Ketersediaan dan penggunaan dataset mengikuti ketentuan masing-masing sumber. Untuk menjalankan notebook, siapkan dataset yang diperlukan dan sesuaikan lokasi file dengan lingkungan pengembangan.

## Struktur Repository

```text
analisis-berita-indonesia/
├── notebooks/
│   ├── 01_data_preprocessing_sentiment.ipynb
│   ├── 02_clustering_topik_berita.ipynb
│   └── 03_eksplorasi_visualisasi.ipynb
├── README.md
└── requirements.txt
```

*Nama notebook di atas merupakan contoh penamaan. Sesuaikan dengan nama dan isi file yang benar-benar diunggah ke repositori.*

## Menjalankan Notebook

1. Unduh atau clone repositori ini.
2. Buka notebook menggunakan Google Colab atau Visual Studio Code dengan dukungan Jupyter Notebook.
3. Instal dependensi yang diperlukan berdasarkan `requirements.txt`.
4. Siapkan dataset yang sesuai dan sesuaikan path file pada notebook.
5. Jalankan setiap notebook sesuai urutan tahapan analisis.

Perlu diperhatikan bahwa beberapa notebook awalnya menggunakan Google Drive sebagai lokasi penyimpanan dataset. Path tersebut perlu disesuaikan jika notebook dijalankan di lingkungan lain.

## Identitas Proyek

**Nama Proyek:** Pengelolaan Big Data Analisis Sentimen dan Tren Topik Berita Online Menggunakan Big Data  
**Kelas:** TI24J  
**Jenis Proyek:** Proyek akademik kelompok

### Anggota Kelompok

1. Mohammad Rifki Indriawan
2. Putri Prisilia Nurul Anwar
3. Rahma Aulia
4. Syifa Nurul Afifah

## Catatan

Proyek ini merupakan proyek akademik yang berfokus pada pengolahan data berita, analisis sentimen, clustering teks, dan visualisasi data. Implementasi setiap tahapan dilakukan sebagai bagian dari kerja kelompok dengan pembagian tugas masing-masing anggota.
