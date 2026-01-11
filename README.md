# Sentiment Analysis ShopeePay Reviews

Proyek ini bertujuan untuk melakukan analisis sentimen terhadap ulasan pengguna aplikasi **ShopeePay** di Google Play Store. Proyek ini mencakup seluruh alur kerja data science, mulai dari scraping data, preprocessing teks, hingga klasifikasi sentimen menggunakan algoritma Machine Learning.

## 📌 Deskripsi Proyek

ShopeePay adalah salah satu layanan dompet digital terbesar di Indonesia. Dengan menganalisis ulasan pengguna, kita dapat memahami tingkat kepuasan pelanggan serta mengidentifikasi masalah teknis atau fitur yang perlu ditingkatkan.

**Tujuan:**

* Melakukan klasifikasi teks menjadi sentimen **Positif**, **Netral**, atau **Negatif**.
* Mengevaluasi performa model Machine Learning dalam memproses bahasa alami (NLP) bahasa Indonesia.

## 📂 Struktur Repositori

* `data/`: Folder berisi dataset mentah (raw) dan hasil pembersihan (cleaned).
* `notebooks/`: Jupyter Notebook yang berisi langkah-langkah analisis.
* `src/`: Skrip Python untuk pemrosesan data.
* `requirements.txt`: Daftar library Python yang diperlukan.
* `README.md`: Dokumentasi proyek.

## 🔧 Teknologi yang Digunakan

* **Bahasa Pemrograman:** Python 3.x
* **Library Utama:**
* `Pandas` & `NumPy` (Manipulasi Data)
* `Scikit-learn` (Machine Learning & Evaluasi)
* `NLTK` / `Sastrawi` (Preprocessing teks bahasa Indonesia)
* `Matplotlib` / `Seaborn` (Visualisasi Data)
* `WordCloud` (Visualisasi kata kunci)



## 🚀 Alur Kerja (Workflow)

1. **Data Collection:** Scraping ulasan pengguna dari Google Play Store menggunakan library `google-play-scraper`.
2. **Preprocessing Teks:**
* Case Folding (mengubah ke huruf kecil).
* Filtering/Cleaning (menghapus angka, simbol, dan URL).
* Tokenizing (pemecahan kalimat menjadi kata).
* Stemming (mengubah kata ke kata dasar menggunakan Sastrawi).
* Stopword Removal (menghapus kata umum yang tidak memiliki makna penting).


3. **Feature Extraction:** Mengubah teks menjadi angka menggunakan metode **TF-IDF**.
4. **Modelling:** Implementasi algoritma (seperti K-Nearest Neighbors, Naive Bayes, atau SVM).
5. **Evaluation:** Mengukur performa model menggunakan *Accuracy*, *Precision*, *Recall*, dan *F1-Score*.

## 📊 Hasil & Visualisasi

*(Opsional: Anda bisa menambahkan gambar WordCloud atau grafik akurasi di sini)*

* Model berhasil mencapai akurasi sebesar `XX%`.
* Sebagian besar ulasan negatif berkaitan dengan isu `[sebutkan isu jika ada, misal: verifikasi wajah atau koneksi]`.

## ⚙️ Cara Menjalankan

1. Clone repositori ini:
```bash
git clone https://github.com/erzafrian/Sentiment-Analysis-ShopeePay.git
cd Sentiment-Analysis-ShopeePay

```


2. Install library yang dibutuhkan:
```bash
pip install -r requirements.txt

```


3. Jalankan Jupyter Notebook untuk melihat proses analisis:
```bash
jupyter notebook notebooks/Sentiment_Analysis.ipynb

```



## 👤 Kontributor

* **Erzafrian** - [GitHub Profile](https://www.google.com/search?q=https://github.com/erzafrian)
