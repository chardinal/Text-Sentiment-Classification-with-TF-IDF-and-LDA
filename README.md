# Text Product Classification with TF-IDF and LDA

Proyek ini membangun pipeline Machine Learning untuk **klasifikasi produk berbasis teks**, menggunakan input berupa **judul dan deskripsi produk**. Sistem akan mengklasifikasikan data tersebut ke dalam kategori berdasarkan model yang sudah dilatih menggunakan **TF-IDF** dan **Linear Discriminant Analysis (LDA)**.

---

## 🌟 Tujuan Proyek

* Mengembangkan sistem klasifikasi produk dari data teks.
* Menerapkan preprocessing teks Bahasa Indonesia.
* Melatih model klasifikasi berbasis LDA.
* Menerapkan prediksi untuk data baru yang diinputkan oleh pengguna.

---

## 📈 Alur Proses Machine Learning

1. **Input Dataset**:

   * Dataset berisi kolom `judul`, `deskripsi`, dan `label/kategori` produk.

2. **Preprocessing Teks**:

   * Case folding (mengubah huruf menjadi huruf kecil)
   * Pembersihan teks dari angka, tanda baca, simbol, dan spasi berlebih
   * Tokenisasi kata
   * Stopword removal
   * Stemming (menggunakan library Sastrawi)

3. **Ekstraksi Fitur**:

   * TF-IDF digunakan untuk mengubah data teks ke representasi numerik

4. **Modeling**:

   * Algoritma klasifikasi: **Linear Discriminant Analysis (LDA)**

5. **Evaluasi Model**:

   * Confusion Matrix
   * Classification Report: Accuracy, Precision, Recall, F1-score

6. **Prediksi Data Baru**:

   * Pengguna dapat memasukkan judul dan deskripsi produk
   * Model memproses dan mengembalikan label kategori hasil klasifikasi

---

## 🪧 Tools dan Teknologi

* Python 3
* Jupyter Notebook
* Scikit-learn
* Pandas, NumPy
* Sastrawi (untuk stemming Bahasa Indonesia)
* TF-IDF Vectorizer
* Matplotlib, Seaborn (visualisasi)

---

## 📊 Struktur Direktori

```
Text-Sentiment-Classification-with-TF-IDF-and-LDA/
│
├── Sentimen Analysis_LDA (Linear Discriminant Analysis).ipynb
├── data/
│   └── dataset.csv (berisi data pelatihan dan label kategori)
├── README.md
└── requirements.txt (opsional)
```

---

## 🚀 Cara Menjalankan

1. **Clone Repository**

```bash
git clone https://github.com/chardinal/Text-Sentiment-Classification-with-TF-IDF-and-LDA.git
cd Text-Sentiment-Classification-with-TF-IDF-and-LDA
```

2. **Jalankan Notebook**

```bash
jupyter notebook
```

3. **Buka dan jalankan**:

   * `Sentimen Analysis_LDA (Linear Discriminant Analysis).ipynb`
   * Jalankan sel-sel dari atas ke bawah sesuai urutan pipeline

---

## 📅 Contoh Input dan Output

**Input:**

```python
judul = "Kamera Mirrorless Resolusi Tinggi"
deskripsi = "Kamera ini dilengkapi sensor CMOS 24MP dan lensa wide angle."
```

**Output:**

```
Kategori Prediksi: Elektronik
```

---

## 📖 Dataset

* Dataset berformat `.csv`
* Minimal berisi kolom:

  * `judul`
  * `deskripsi`
  * `label` (kategori produk)

---

## 📁 Contoh Dataset

| judul                 | deskripsi                                                          | label      |
| --------------------- | ------------------------------------------------------------------ | ---------- |
| Sepatu Olahraga Pria  | Sepatu ringan dan nyaman digunakan untuk olahraga harian           | Fashion    |
| Laptop Gaming Ryzen 7 | Laptop dengan prosesor Ryzen 7 dan GPU RTX 3060 untuk gaming berat | Elektronik |


Jika proyek ini bermanfaat, silakan berikan bintang ⭐ untuk mendukung pengembangan lebih lanjut.
