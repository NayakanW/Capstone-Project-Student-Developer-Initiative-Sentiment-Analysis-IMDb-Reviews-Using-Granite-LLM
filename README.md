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

## ⚙️ Instalasi
Jalankan di Google Colab atau lokal Python environment.

```bash
!pip install langchain_community replicate pandas scikit-learn matplotlib
