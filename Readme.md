# Klasifikasi Berita Bahasa Indonesia (News Classification) 📰
Tugas Kelompok - Klasifikasi Berita 

## 👥 Anggota Kelompok
* Ahmad Hamizan - Informatics Engineering
* Ahmad Yudistira Ramdhany - Informatics Engineering
* Muhammad Rizqi Nurrohmat - Informatics Engineering
* Muhammad Zakri Alfiansyah - Informatics Engineering
* Razan Muhammad Ihsan Rismawandi - Informatics Engineering

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk mengklasifikasikan kategori berita (misal: Politik, Ekonomi, Olahraga, Teknologi) menggunakan teknik Natural Language Processing (NLP). Kami membandingkan performa berbagai algoritma Machine Learning dan teknik ekstraksi fitur untuk mendapatkan akurasi terbaik.

---

## 🛠️ Alur Pengerjaan (Pipeline)

### 1. Data Collection
* **Dataset**: Menggunakan dataset berita Bahasa Indonesia (Kaggle/Scraping).
* **Ukuran**: > 10.000 data point.

### 2. Text Preprocessing
Proses pembersihan teks mentah agar siap diolah oleh model:
* **Case Folding**: Mengubah semua teks menjadi huruf kecil.
* **Tokenization**: Memecah kalimat menjadi kata-kata tunggal.
* **Stopword Removal**: Menghapus kata umum yang tidak memiliki makna penting (dan, yang, di, dll).
* **Stemming**: Mengubah kata berimbuhan menjadi kata dasar menggunakan library Sastrawi.

### 3. Feature Extraction (Wajib 2)
Kami membandingkan dua metode representasi teks:
1. **TF-IDF (Term Frequency - Inverse Document Frequency)**
2. **Word Embedding (Word2Vec / GloVe)**

### 4. Modeling (Wajib 3 Model)
Algoritma yang digunakan dalam eksperimen:
1. **Naive Bayes** (Baseline)
2. **Logistic Regression**
3. **Support Vector Machine (SVM)**

### 5. Evaluasi & Perbandingan
Analisis performa model dilakukan berdasarkan metrik:
* **Accuracy, Precision, Recall, dan F1-Score.**
* Perbandingan performa **TF-IDF vs Word Embedding**.

---

## 🚀 Deployment
Proyek ini dideploy menggunakan **Gradio** untuk antarmuka pengguna yang sederhana. Kamu bisa memasukkan teks berita, dan model akan memprediksi kategori berita tersebut secara real-time.

---

## 📂 Struktur Folder
```text
.
├── data/               # Dataset mentah & bersih
├── notebooks/          # File .ipynb (Preprocessing & Modeling)
├── models/             # Saved model (.pkl / .h5)
├── src/                # Script deployment Gradio
└── README.md