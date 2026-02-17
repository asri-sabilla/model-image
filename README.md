# 🕳️ Pothole Segmentation — Computer Vision Project

**Semantic Segmentation of Road Surface Damage using U-Net**

## 📌 Project Overview
Project ini dikembangkan dalam rangka **Data Science Competition – ARA 7.0** yang diselenggarakan oleh **Institut Teknologi Sepuluh Nopember**.
Tujuan utama project adalah membangun **model segmentasi lubang jalan (pothole segmentation)** dari citra permukaan jalan menggunakan pendekatan **Deep Learning**.

Model dirancang untuk mampu **mengenali dan menandai area lubang jalan secara presisi** pada berbagai kondisi, seperti:

* Perbedaan sudut pengambilan gambar
* Variasi pencahayaan
* Tekstur jalan yang beragam
* Ukuran lubang jalan yang bervariasi

Project ini merepresentasikan penerapan **Artificial Intelligence dan Computer Vision** untuk mendukung **keselamatan dan pemeliharaan infrastruktur jalan**.

---

## 🎯 Problem Statement

Kerusakan jalan seperti lubang jalan sering kali sulit terdeteksi secara manual dan memerlukan inspeksi visual yang memakan waktu serta biaya tinggi.

Tantangan utama:

* Variasi kondisi lingkungan (cahaya, sudut kamera, tekstur jalan)
* Perbedaan ukuran dan bentuk lubang jalan
* Kebutuhan segmentasi area yang presisi, bukan hanya klasifikasi gambar

---

## 🎯 Objectives

* Membangun model **semantic segmentation** untuk mendeteksi area lubang jalan
* Menggunakan **arsitektur U-Net** untuk memprediksi mask lubang jalan dari citra jalan
* Mengevaluasi performa model pada data uji dengan kondisi yang bervariasi
* Menghasilkan model AI yang dapat digunakan sebagai dasar **sistem deteksi kerusakan jalan otomatis**

---

## 🛠️ Tech Stack & Workflow

### 1️⃣ Data Understanding & Preparation

* Dataset berupa **pasangan citra jalan dan mask ground truth**
* Mask menunjukkan area lubang jalan pada setiap gambar
* Proses:

  * Data loading
  * Image preprocessing
  * Penyesuaian ukuran citra dan mask

---

### 2️⃣ Data Preprocessing

* Normalisasi citra
* Penyesuaian format mask segmentasi
* Penanganan variasi pencahayaan dan sudut pengambilan gambar
* (Opsional) Data augmentation untuk meningkatkan generalisasi model

---

### 3️⃣ Modeling — U-Net (Deep Learning)

* Arsitektur utama: **U-Net**
* Digunakan untuk **semantic segmentation** pada citra jalan
* Proses:

  * Training model menggunakan data latih
  * Validasi performa selama proses pelatihan
  * Penyesuaian parameter untuk meningkatkan hasil segmentasi

---

### 4️⃣ Evaluation & Prediction

* Evaluasi model berdasarkan kualitas hasil segmentasi
* Visualisasi hasil prediksi berupa **overlay mask lubang jalan pada citra asli**
* Model diuji pada data test untuk memprediksi area lubang jalan yang belum pernah dilihat sebelumnya

---

## 📂 Repository Structure

```
├── data/
│   ├── train/                 # Citra dan mask untuk data latih
│   └── test/                  # Citra untuk data uji
├── notebooks/
│   ├── 01_eda.ipynb            # Eksplorasi data dan visualisasi awal
│   └── 02_modeling_unet.ipynb  # Training dan evaluasi model U-Net
├── src/
│   ├── preprocessing.py       # Preprocessing citra dan mask
│   ├── model_unet.py           # Arsitektur model U-Net
│   └── train.py                # Proses training dan evaluasi
├── assets/
│   ├── sample_prediction.png  # Contoh hasil segmentasi
└── README.md
```

---

## 🔍 Key Highlights

* Menggunakan **Deep Learning (U-Net)** untuk segmentasi citra
* Mampu mendeteksi lubang jalan pada berbagai kondisi lingkungan
* Project berbasis **Computer Vision & AI** dengan pendekatan end-to-end
* Merepresentasikan workflow **data science kompetisi berbasis Kaggle**

---

## 📌 Potential Impact

* Mendukung sistem **pemeliharaan jalan berbasis AI**
* Mengurangi ketergantungan pada inspeksi manual
* Dapat dikembangkan lebih lanjut untuk:

  * Smart City
  * Sistem monitoring jalan otomatis
  * Integrasi dengan GIS atau dashboard infrastruktur

---

## 👤 Author

**Asri Sabilla Putri**
Data Science & Machine Learning Enthusiast
🔗 LinkedIn: [https://linkedin.com/in/asrisabilla](https://linkedin.com/in/asrisabilla)
🌐 Portfolio: [https://portofolio-asri.netlify.app](https://portofolio-asri.netlify.app)
