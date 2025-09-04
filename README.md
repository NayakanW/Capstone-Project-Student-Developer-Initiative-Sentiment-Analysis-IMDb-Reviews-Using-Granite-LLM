# 🎬 Analisis Sentimen Ulasan Film IMDb dengan Granite API

Proyek ini bertujuan untuk melakukan **analisis sentimen** terhadap ulasan film dari dataset **IMDb Movie Reviews** menggunakan **LLM Granite 3.3 (via Replicate API)**.

---

## 🚀 Fitur Utama
- Memuat dataset `IMDB Dataset.csv` (50.000 review film dengan label sentiment).
- Mengambil sampel 100 review untuk evaluasi (hemat biaya token).
- Menggunakan **Granite LLM** untuk klasifikasi sentimen (Positive / Negative).
- Membandingkan prediksi Granite dengan label asli untuk menghitung **akurasi**.
- Menampilkan hasil berupa:
  - Akurasi klasifikasi
  - Confusion matrix
  - Distribusi prediksi (bar chart)

---

## 📂 Struktur Proyek
.

├── IMDB Dataset.csv        # Dataset utama  
├── granite_sentiment.ipynb # Notebook utama (pipeline)  
├── README.md               # Dokumentasi  
└── requirements.txt        # Dependensi Python  

---

## 📊 Sumber Dataset
Dataset IMDB Dataset.csv dapat di download melalui link berikut:
https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews

---

## ⚙️ Instalasi
Jalankan di Google Colab atau lokal Python environment.

```bash
!pip install langchain_community replicate pandas scikit-learn matplotlib

```
---

## 🔑 API Token
Daftarkan akun di Replicate untuk mendapatkan API Token.

Set token di Colab:
```bash
import os
os.environ["REPLICATE_API_TOKEN"] = "YOUR_API_TOKEN"

```

