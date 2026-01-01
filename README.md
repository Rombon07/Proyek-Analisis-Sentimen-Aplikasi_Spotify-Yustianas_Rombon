# 🎵 Spotify App Reviews Sentiment Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![Google Play Scraper](https://img.shields.io/badge/Google_Play_Scraper-Scraping-green?style=for-the-badge)
![NLTK](https://img.shields.io/badge/NLTK-NLP-yellow?style=for-the-badge)

Repository ini berisi proyek **End-to-End Sentiment Analysis** terhadap ulasan aplikasi **Spotify** di Google Play Store. Proyek ini mencakup tahapan pengambilan data (scraping) hingga prediksi sentimen menggunakan Machine Learning/Deep Learning.

---

## 📋 Tentang Proyek

Tujuan dari proyek ini adalah untuk menganalisis opini pengguna terhadap aplikasi Spotify, apakah cenderung **Positif** atau **Negatif**.

Alur kerja proyek:
1.  **Data Scraping:** Mengambil ulasan nyata dari Google Play Store.
2.  **Data Preprocessing:** Membersihkan teks (menghapus stopwords, cleaning text) menggunakan `NLTK`.
3.  **Modeling:** Melatih model (menggunakan TensorFlow/Scikit-Learn) untuk mengklasifikasikan sentimen.
4.  **Prediction:** Menguji model dengan kalimat baru.

---

## 📂 Struktur Repository

Berikut adalah penjelasan fungsi dari setiap file dalam repository ini:

### 1. 🕵️‍♂️ Scraping Data
* **File:** `scraping.ipynb`
* **Deskripsi:** Script ini menggunakan library `google-play-scraper` untuk mengambil ribuan ulasan terbaru dari aplikasi Spotify.
* **Output:** Menghasilkan file raw data bernama `dataset_spotify_RAW.csv`.

### 2. 📊 Dataset
* **File:** `dataset_spotify_RAW.csv`
* **Deskripsi:** Kumpulan data mentah hasil scraping.
* **Kolom:**
    * `Teks`: Isi ulasan pengguna.
    * `Bintang`: Rating yang diberikan (1-5).
    * `Tanggal`: Waktu ulasan diberikan.

### 3. 🧠 Analisis & Pemodelan
* **File:** `Analisis_sentimen.ipynb`
* **Deskripsi:** Notebook utama untuk analisis sentimen.
* **Proses:**
    * Load dataset.
    * Preprocessing (Tokenisasi, Stopwords removal).
    * Training Model (TensorFlow/Keras).
    * Evaluasi Akurasi.
    * **Demo Prediksi:** Memasukkan kalimat manual untuk dicek sentimennya.

### 4. ⚙️ Dependencies
* **File:** `requirements.txt`
* **Deskripsi:** Daftar library yang digunakan dalam proyek ini.

---

## 🚀 Cara Menjalankan

1.  **Clone Repository**
    ```bash
    git clone https://github.com/Rombon07/Proyek-Analisis-Sentimen-Aplikasi_Spotify-Yustianas_Rombon.git
    ```

2.  **Install Library**
    Pastikan kamu sudah menginstall semua library yang dibutuhkan:
    ```bash
    pip install -r requirements.txt
    ```
    *Library utama: `pandas`, `numpy`, `google-play-scraper`, `nltk`, `tensorflow`, `matplotlib`, `seaborn`.*

3.  **Jalankan Notebook**
    * Buka `scraping.ipynb` jika ingin memperbarui data ulasan terbaru.
    * Buka `Analisis_sentimen.ipynb` untuk melatih model dan melihat hasil prediksi.

---

## 🧪 Contoh Hasil Prediksi

Berdasarkan output model di `Analisis_sentimen.ipynb`:

| Input Ulasan | Prediksi Sentimen | Probabilitas |
| :--- | :---: | :---: |
| *"aplikasinya bagus banget, suka deh! lancar jaya"* | **Positif** | 89.86% |
| *"Sudah cukup bagus, koleksi lagunya lengkap."* | **Positif** | 98.15% |

---

## 📈 Tools yang Digunakan

* **Google Play Scraper**: Untuk mengambil data ulasan secara real-time.
* **Pandas & NumPy**: Untuk manipulasi dan analisis data tabular.
* **Matplotlib & Seaborn**: Untuk visualisasi distribusi rating dan sentimen.
* **NLTK**: Untuk pemrosesan bahasa alami (Natural Language Processing).
* **TensorFlow / Scikit-Learn**: Framework untuk membangun model klasifikasi.

---

**Author:** Yustianas Rombon  
**Program:** Dicoding - Belajar Fundamental deep learning
