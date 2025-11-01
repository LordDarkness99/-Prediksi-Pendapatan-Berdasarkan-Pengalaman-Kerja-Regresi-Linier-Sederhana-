# 💼 Prediksi Pendapatan Berdasarkan Pengalaman Kerja — Regresi Linier Sederhana

Proyek ini merupakan implementasi **Machine Learning dasar (Regresi Linier Sederhana)** untuk memprediksi **pendapatan seseorang (dalam Rupiah)** berdasarkan **lama pengalaman kerja (dalam tahun)**.  
Proyek ini terinspirasi dari *Model Representation* pada kursus Machine Learning oleh Andrew Ng, dan disesuaikan dengan konteks Indonesia.

---

## 📘 Deskripsi Proyek

Tujuan utama proyek ini adalah memahami bagaimana model regresi linier dapat menemukan hubungan matematis antara dua variabel:

\[
f_{w,b}(x) = w \times x + b
\]

Di mana:
- `x` = pengalaman kerja (tahun)  
- `f_{w,b}(x)` = pendapatan (Rupiah)  
- `w` = kemiringan garis (berapa besar kenaikan pendapatan per tahun pengalaman)  
- `b` = bias/intersep (pendapatan awal tanpa pengalaman)

---

## ⚙️ Fitur Utama
- Menggunakan **NumPy** untuk komputasi matematis  
- Menggunakan **Matplotlib** untuk visualisasi data dan hasil model  
- Implementasi **manual dari gradient descent** tanpa library ML tambahan  
- Satuan disesuaikan dengan konteks Indonesia:
  - Pengalaman kerja → Tahun  
  - Pendapatan → Rupiah (Rp)

---

## 📊 Dataset Contoh

| Pengalaman (Tahun) | Pendapatan (Rp)   |
|---------------------|------------------:|
| 1                   | 4,000,000         |
| 3                   | 7,000,000         |
| 5                   | 11,000,000        |
| 7                   | 14,000,000        |
| 9                   | 17,000,000        |

Model akan belajar dari data sederhana ini untuk memperkirakan seberapa besar pengaruh pengalaman terhadap pendapatan seseorang.

---

## 🧠 Algoritma yang Digunakan

1. **Model Linier**  
   \[
   f_{w,b}(x) = w \times x + b
   \]

2. **Fungsi Biaya (Cost Function)**  
   Menggunakan *Mean Squared Error (MSE)*:
   \[
   J(w,b) = \frac{1}{2m} \sum_{i=1}^{m}(f_{w,b}(x^{(i)}) - y^{(i)})^2
   \]

3. **Gradient Descent**  
   Algoritma untuk mencari nilai terbaik dari `w` dan `b` secara iteratif agar error sekecil mungkin.

---

## 🚀 Cara Menjalankan

### Persyaratan
Pastikan Python dan library berikut sudah terpasang:
```bash
pip install numpy matplotlib
