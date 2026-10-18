#  Automated Credit Risk Classification & Machine Learning Pipeline

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Scikit-Learn](https://img.shields.io/badge/ML-Scikit--Learn-F7931E)
![Pandas](https://img.shields.io/badge/Data-Pandas-150458)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📋 Studi Kasus: Sistem Klasifikasi Kelayakan Kredit Nasabah Bank

### 1. Latar Belakang Masalah
Dalam sektor perbankan dan lembaga keuangan, penetapan kelayakan permohonan pinjaman/kredit (*Credit Risk Assessment*) secara manual memerlukan waktu lama dan rawan terkena bias subyektif manusia. Jika bank salah memberikan kelayakan kepada nasabah berisiko tinggi, hal ini dapat memicu timbulnya kredit macet (*Non-Performing Loan / NPL*).

### 2. Solusi Machine Learning & Implementation Workflow
Mengacu pada materi **Assoc. Prof. Ts. Dr. Taniza Binti Tajuddin** (*UiTM Kedah, Malaysia*) dalam *Informatics Practitioner Lecture Series*, pergeseran dari pemrograman tradisional (*rule-based*) menuju **Machine Learning** memungkinkan sistem belajar secara mandiri dari pola data historis nasabah.

Proyek ini menerapkan **Supervised Machine Learning (Supervised Classification)** untuk memprediksi secara otomatis apakah permohonan kredit nasabah diterima (`Disetujui / Layak`) atau ditolak (`Ditolak / Berisiko`).

---

## ⚙️ 6-Tahap Alur Kerja ML (ML Workflow)

Proyek ini menerapkan 6 tahapan *End-to-End ML Pipeline* standar industri:

1. **Data Collection:** Pembuatan dataset tabular yang mencakup atribut nasabah (Usia, Pendapatan, Skor Kredit, Jumlah Pinjaman, Status Pekerjaan, dan Hutang Berjalan).
2. **Data Pre-processing:** Penanganan data kualitatif menggunakan *Label Encoding* dan normalisasi variabel numerik menggunakan *StandardScaler*.
3. **Data Splitting:** Pembagian dataset secara terstrata dengan rasio **70% Data Training** dan **30% Data Testing**.
4. **Model Selection & Training:** Membandingkan dua algoritma berbasis pohon keputusan, yaitu **Decision Tree** dan **Random Forest Classifier**.
5. **Model Evaluation:** Evaluasi mendalam menggunakan metrik *Accuracy*, *Precision*, *Recall*, *F1-Score*, serta visualisasi *Confusion Matrix*.
6. **Deployment & Model Persistence:** Penyimpanan model hasil *fine-tuning* ke dalam format `.pkl` (Pickle) agar siap diintegrasikan dengan aplikasi web atau API backend.

---

## 📊 Metrik Evaluasi Model

| Metrik Evaluasi | Deskripsi / Fungsi |
| :--- | :--- |
| **Accuracy** | Mengukur persentase total prediksi yang benar secara keseluruhan. |
| **Precision** | Mengukur ketepatan model ketika memprediksi nasabah layak kredit. |
| **Recall** | Mengukur kemampuan model menemukan seluruh nasabah yang berisiko. |
| **F1-Score** | Rata-rata harmonis antara *Precision* dan *Recall*. |
| **Confusion Matrix** | Tabel matriks untuk melihat detail *True Positive*, *False Positive*, *True Negative*, dan *False Negative*. |

---

## 📁 Struktur Repositori

```
├── ML_Credit_Risk.ipynb # Jupyter / Google Colab Notebook (Kode Utama)
├── credit_risk_dataset.csv       # Dataset mentah nasabah (CSV)
├── credit_risk_model.pkl         # Model ML terpisah hasil ekspor (Random Forest)
├── scaler.pkl                    # File scaler fitur (StandardScaler)
└── README.md                     # Dokumentasi utama proyek
```

---

## 🚀 Cara Menjalankan di Google Colab

1. Unduh file `ML_Credit_Risk.ipynb` dari repositori ini atau buat notebook baru di [Google Colab](https://colab.research.google.com/).
2. Jalankan sel (*cells*) kode secara berurutan dari **Sel 1 hingga Sel 7**.
3. Sel 7 akan otomatis memuat dan mengunduh file dataset (`credit_risk_dataset.csv`), model terlatih (`credit_risk_model.pkl`), dan file *scaler* ke komputer Anda.

---

## 👥 Referensi & Kredit
* **Pemateri:** Assoc. Prof. Ts. Dr. Taniza Binti Tajuddin (*Universiti Teknologi MARA / UiTM Kedah, Malaysia*).
* **Materi:** *"Introduction to Machine Learning"* - Informatics Practitioner Lecture Series, Universitas Bengkulu.
