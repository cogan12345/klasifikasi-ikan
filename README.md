---
title: Klasifikasi Kesegaran Ikan
emoji: 🐟
colorFrom: blue
colorTo: green
sdk: streamlit
sdk_version: 1.32.0
app_file: app.py
pinned: false
python_version: "3.11"
---

# 🐟 Klasifikasi Kesegaran Ikan — Streamlit App

Aplikasi web klasifikasi kesegaran ikan menggunakan CNN MobileNetV2.

---

## 📁 Struktur Folder

```
project/
├── app.py               ← file utama aplikasi Streamlit
├── model_final.keras    ← model hasil training (copy dari output notebook)
├── requirements.txt     ← daftar library yang dibutuhkan
└── README.md
```

---

## 🚀 Cara Menjalankan (Lokal)

### 1. Install Library
```bash
pip install -r requirements.txt
```

### 2. Jalankan Aplikasi
```bash
streamlit run app.py
```

Aplikasi akan terbuka otomatis di browser: **http://localhost:8501**

---

## ☁️ Deploy ke Hugging Face Spaces (Gratis)

1. Buat akun di **https://huggingface.co**
2. Buka **https://huggingface.co/new-space**
3. Pilih SDK: **Streamlit**
4. Klik **Create Space**
5. Di halaman Space → tab **Files** → upload semua file dari repo ini
6. App otomatis live!

---

## 📌 Catatan

- Model menerima input gambar berukuran **224 × 224 piksel** (diproses otomatis)
- Output: **Fresh** (segar) atau **Not Fresh** (tidak segar)
- Model dilatih pada 3 jenis ikan: Nila, Kembung, Tuna
