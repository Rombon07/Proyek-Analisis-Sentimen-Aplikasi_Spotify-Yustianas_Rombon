# Proyek Analisis Sentimen Aplikasi Spotify 🎵

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📋 Deskripsi Proyek

Proyek ini bertujuan untuk melakukan **Analisis Sentimen** terhadap ulasan pengguna aplikasi **Spotify** (bersumber dari Google Play Store).

Tujuan utama dari analisis ini adalah untuk memahami persepsi pengguna terhadap aplikasi Spotify dengan mengklasifikasikan ulasan mereka ke dalam kategori sentimen (misalnya: **Positif** atau **Negatif**). Wawasan ini berguna untuk mengetahui fitur apa yang disukai pengguna dan keluhan apa yang paling sering muncul.

## 🚀 Fitur & Metodologi

Proyek ini mencakup langkah-langkah *end-to-end* dalam pemrosesan data teks (NLP):

1.  **Pengumpulan Data (Data Collection):** Menggunakan dataset ulasan aplikasi Spotify.
2.  **Preprocessing Data:**
    * *Cleaning* (Menghapus tanda baca, angka, emoji).
    * *Case Folding* (Mengubah teks menjadi huruf kecil).
    * *Stopword Removal* (Menghapus kata umum yang tidak bermakna).
    * *Stemming/Lemmatization* (Mengubah kata ke bentuk dasar).
3.  **Ekstraksi Fitur (Feature Extraction):** Mengubah teks menjadi angka menggunakan metode seperti **TF-IDF** atau **Bag of Words**.
4.  **Pemodelan (Modeling):** Melatih model Machine Learning (misalnya: Naive Bayes, SVM, atau Random Forest) untuk klasifikasi sentimen.
5.  **Evaluasi:** Mengukur performa model menggunakan metrik *Accuracy*, *Precision*, *Recall*, dan *F1-Score*.

## 🛠️ Teknologi yang Digunakan

* **Bahasa Pemrograman:** Python
* **Library Pengolahan Data:** Pandas, NumPy
* **Visualisasi Data:** Matplotlib, Seaborn, WordCloud
* **Natural Language Processing (NLP):** NLTK / Sastrawi (jika ulasan bahasa Indonesia) / Scikit-learn
* **Machine Learning:** Scikit-Learn

## 📂 Struktur File

```text
Proyek-Analisis-Sentimen-Aplikasi_Spotify-Yustianas_Rombon/
├── data/                   # Folder untuk menyimpan dataset (csv/xlsx)
├── notebooks/              # File Jupyter Notebook (.ipynb) berisi analisis & kode
├── images/                 # Hasil visualisasi (grafik, wordcloud)
├── README.md               # Dokumentasi proyek
└── requirements.txt        # Daftar library yang diperlukan
