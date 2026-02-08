# Integrated AI Approach for Telecommunication Customer Churn Analysis 📡📊

Proyek ini merupakan studi komparatif penggunaan berbagai algoritma **Supervised Learning** untuk memprediksi *churn* pelanggan pada industri telekomunikasi. Fokus utama proyek adalah menerapkan alur kerja Data Science yang lengkap, mulai dari penanganan data yang tidak seimbang (*imbalanced data*) hingga interpretasi fitur untuk mendukung strategi retensi bisnis.

## 🚀 Fitur Utama & Metodologi
- **Kerangka Kerja PEAS:** Analisis sistem cerdas berdasarkan *Performance, Environment, Actuators,* dan *Sensors*.
- **Data Preprocessing & Cleaning:**
  - Pembersihan atribut yang tidak relevan (seperti *Churn Reason* dan *Churn Score*) untuk mencegah kebocoran data (*data leakage*).
  - Transformasi variabel kategorikal menggunakan *Binary* dan *One-Hot Encoding*.
  - Penanganan data tidak seimbang menggunakan **SMOTE** (Synthetic Minority Oversampling Technique) untuk meningkatkan akurasi deteksi pada kelompok pelanggan yang berhenti.
  - Standarisasi fitur menggunakan **StandardScaler** untuk optimasi algoritma yang sensitif terhadap skala data.
- **Komparasi Algoritma Supervised:** Studi mendalam menggunakan tiga model utama: **Decision Tree (CART)**, **Naive Bayes**, dan **Artificial Neural Network (MLP)**.



## 🛠️ Tech Stack & Libraries
- **Bahasa Pemrograman:** Python
- **Library Utama:**
  - **Pandas & NumPy:** Manipulasi dan pembersihan dataset.
  - **Scikit-Learn:** Pembangunan model klasifikasi dan evaluasi metrik (Accuracy, Recall, F1-Score).
  - **Matplotlib & Seaborn:** Visualisasi data, Confusion Matrix, dan Feature Importance.
  - **Imbalanced-learn:** Implementasi teknik *oversampling* SMOTE.

## 📈 Hasil Evaluasi Model
Berdasarkan eksperimen pada dataset Telco Customer Churn (~4,230 data), berikut adalah perbandingan performa ketiga algoritma:

| Metric | Decision Tree | Naive Bayes | ANN (MLP) |
| :--- | :---: | :---: | :---: |
| **Overall Accuracy** | 80% | 79% | 80% |
| **Recall (Churn/Class 1)** | 0.68 | **0.82** | 0.79 |
| **Balanced Accuracy** | 76.04% | 79.80% | 79.78% |

**Analisis Teknis:** **Naive Bayes** terbukti paling efektif untuk tujuan retensi karena memiliki nilai **Recall tertinggi (82%)**, yang berarti mampu mendeteksi 82% pelanggan yang benar-benar akan berhenti. Sementara itu, **ANN** memberikan performa yang paling stabil dan seimbang di seluruh kategori penilaian.

## 💡 Key Business Insights
- **Faktor Kontrak:** Tipe kontrak adalah prediktor churn paling kuat. Pelanggan dengan kontrak **Month-to-month** memiliki risiko berhenti paling tinggi, sementara kontrak dua tahun adalah indikator loyalitas yang sangat kuat.
- **Risiko Layanan:** Pengguna layanan **Fiber Optic** ditemukan memiliki tingkat churn yang lebih tinggi dibandingkan pengguna DSL atau tanpa internet.
- **Relasi Sosial:** Jumlah referensi pelanggan (*Number of Referrals*) berkorelasi positif dengan loyalitas; pelanggan yang memberikan referensi cenderung bertahan lebih lama.



## 📂 Struktur Repositori
- `Final Report.pdf`: Dokumentasi teknis lengkap mengenai metodologi dan hasil riset.
- `churn_analysis.ipynb`: Notebook Jupyter berisi seluruh kode pemrograman (Cleaning, Modeling, Evaluation).
- `visualizations/`: Kumpulan gambar Confusion Matrix dan visualisasi Decision Tree.

## 📝 Tim Pengembang (Sains Data UNESA)
- **Abdullah Al-Firdaus Nuzula** (24031554008)
- **Fio Ulaa' Octriyanti** (24031554030)
- **Muhammad Rafi Fahrezi** (24031554100)

**Dosen Pengampu:** Riskyana Dewi Intan Puspitasari, M.Kom & Kartika Chandra Dewi, S.Si, M.Si.
