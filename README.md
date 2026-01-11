# 📊 Sentiment Analysis ShopeePay Reviews

## 🔍 Ringkasan Proyek

Proyek ini bertujuan melakukan **analisis sentimen terhadap ulasan pengguna aplikasi ShopeePay** yang diambil dari Google Play Store. Dengan memanfaatkan teknik *Natural Language Processing (NLP)* dan *Machine Learning*, teks ulasan diklasifikasikan menjadi sentimen **positif**, **netral**, atau **negatif** untuk memahami persepsi pengguna terhadap layanan e-wallet ini.

ShopeePay menjadi bagian penting ekosistem dompet digital di Indonesia dengan jutaan pengguna, sehingga analisis sentimen menjadi dasar evaluasi kepuasan dan pengalaman pengguna. 

---

## 🧠 Tujuan Utama

* 🗂️ **Klasifikasi sentimen teks ulasan** login ShopeePay
* 📈 **Evaluasi performa model Machine Learning** untuk NLP
* 🧩 **Memetakan respons pengguna** terhadap fitur dan layanan ShopeePay
* 🛠️ **Menjadi basis pengembangan sistem rekomendasi dan monitoring feedback pengguna** 

---

## 📁 Struktur Repositori

```
Sentiment-Analysis-ShopeePay/
├── [Pelatihan_Model]/                # Notebook training dan evaluasi model
│   └── Analisis_Sentimen_ShopeePay.ipynb
├── [Scraping]/                       # Notebook scraping ulasan
│   └── Analisis_Sentimen_ShopeePay.ipynb
├── shopeepay_reviews4.csv            # Dataset ulasan ShopeePay
├── requirements.txt                  # Ketergantungan Python
├── README.md                         # Dokumentasi proyek
```

---

## 🧰 Teknologi yang Digunakan

| Komponen              | Tools / Library                |               |
| --------------------- | ------------------------------ | ------------- |
| Bahasa Pemrograman    | Python 3.x                     |               |
| NLP & Text Processing | NLTK, Sastrawi                 |               |
| Feature Engineering   | TF-IDF Vectorizer              |               |
| Machine Learning      | Scikit-Learn                   |               |
| Visualisasi           | Matplotlib, Seaborn, WordCloud |               |
| Dataset               | CSV ulasan pengguna ShopeePay  | ([GitHub][1]) |

---

## 🧩 Alur Kerja Analisis (Workflow)

1. **Pengumpulan Data (Scraping)**

   * Mengambil ulasan pengguna ShopeePay dari Google Play Store. 

2. **Pembersihan & *Preprocessing* Teks**

   * Case folding (huruf kecil), pembersihan simbol, tokenisasi, *stopword removal*, dan *stemming* menggunakan *Sastrawi* serta *NLTK*. 

3. **Ekstraksi Fitur**

   * Mengubah teks menjadi representasi numerik melalui TF-IDF. 

4. **Pemodelan Sentimen**

   * Melatih *Machine Learning* untuk klasifikasi teks menjadi sentimen. 

5. **Evaluasi Model**

   * Mengukur metrik seperti *accuracy*, *precision*, *recall*, dan *F1-score* untuk menilai kualitas klasifikasi model. 

---

## 🚀 Cara Menjalankan Proyek

### 📌 1. Clone Repository

```bash
git clone https://github.com/erzafrian/Sentiment-Analysis-ShopeePay.git
cd Sentiment-Analysis-ShopeePay
```

### 📌 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 📌 3. Buka Jupyter Notebook

Jalankan notebook untuk melihat langkah-langkah scraping, preprocessing, dan modelling:

```bash
jupyter notebook [Pelatihan_Model]/Analisis_Sentimen_ShopeePay.ipynb
```

---

## 📈 Hasil & Insight

Proyek ini menghasilkan:

* Model klasifikasi teks uji dengan performa evaluasi yang dapat dibandingkan melalui metrik akurasi dan *confusion matrix*.
* Visualisasi kata kunci menggunakan WordCloud untuk insight umum ulasan negatif/positif.
