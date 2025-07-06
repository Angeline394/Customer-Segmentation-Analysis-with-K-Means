# 📊 Analisis Segmentasi Pelanggan Ritel dengan K-Means Clustering

Halo! Selamat datang di proyek analisis data pelanggan ritel. Di sini, saya mencoba mengelompokkan pelanggan berdasarkan pola belanja mereka menggunakan algoritma **K-Means Clustering**. Tujuannya adalah supaya bisnis bisa lebih mengenali tipe-tipe pelanggannya dan mengambil keputusan yang lebih tepat, terutama untuk strategi pemasaran dan pelayanan pelanggan.

---

## 🎯 Tujuan Proyek

Bisnis ritel sering menghadapi tantangan dalam memahami kebutuhan dan perilaku pelanggan. Melalui segmentasi, kita bisa membagi pelanggan ke dalam beberapa kelompok berdasarkan kemiripan kebiasaan mereka, misalnya dari frekuensi belanja, total belanja, atau jumlah produk yang dibeli.

Dengan teknik **K-Means Clustering**, proyek ini bertujuan untuk:

- Mengidentifikasi kelompok pelanggan dengan karakteristik yang berbeda-beda.
- Memberikan insight yang bisa digunakan untuk kampanye marketing yang lebih terarah.
- Membantu bisnis dalam merancang program loyalitas atau penawaran khusus.
- Meningkatkan retensi dan pengalaman pelanggan secara keseluruhan.

---

## 🔍 Alur Analisis

### 1. Pengumpulan Data
Dataset yang digunakan berisi data transaksi pelanggan pada sebuah toko ritel. Data bisa dalam bentuk `.csv` atau `.xlsx`.

### 2. Pembersihan Data
Tahap ini meliputi:

- Menghapus data kosong (missing values).
- Menghapus data duplikat.
- Memastikan bahwa semua data relevan dan layak dianalisis.

### 3. Eksplorasi Data (EDA - Exploratory Data Analysis)
Langkah ini dilakukan untuk memahami isi dan struktur data lebih dalam. Beberapa hal yang dilakukan di tahap ini:

- Melihat distribusi data dan outlier.
- Menyusun ringkasan statistik dari fitur utama.
- Membuat grafik visualisasi awal dengan Seaborn dan Matplotlib.

### 4. Pra-pemrosesan Data
Agar data bisa diproses oleh algoritma K-Means, dilakukan beberapa transformasi:

- **Feature Engineering**: membuat kolom baru dari data yang sudah ada jika dibutuhkan.
- **Standardisasi Data**: menggunakan `StandardScaler` agar semua fitur berada dalam skala yang sama.

### 5. Penentuan Jumlah Klaster
Sebelum menjalankan K-Means, kita perlu menentukan jumlah klaster terbaik. Ini dilakukan menggunakan:

- **Metode Elbow**
- **Silhouette Score**

Tujuannya agar klaster yang terbentuk benar-benar representatif terhadap data.

### 6. Implementasi K-Means Clustering
Setelah jumlah klaster ditentukan, dilakukan proses pengelompokan pelanggan dengan algoritma K-Means dari library `scikit-learn`.

### 7. Visualisasi Klaster
Hasil klaster divisualisasikan dalam bentuk grafik 2D dan 3D (opsional), menggunakan:

- `Matplotlib`
- `Seaborn`
- `Plotly` (untuk visualisasi interaktif)

### 8. Analisis dan Interpretasi
Setelah terbentuk klaster, dilakukan analisis terhadap masing-masing kelompok pelanggan:

- Siapa saja pelanggan dalam setiap klaster?
- Apa karakteristik khas tiap klaster?
- Apa strategi bisnis yang cocok diterapkan untuk tiap segmen?

## 📊 Dashboard Segmentasi Pelanggan

Visualisasi hasil segmentasi pelanggan menggunakan RFM dan K-Means:

![Dashboard K-Means](images/Customer_segmentation_dashboard.png)




## 🛠️ Tools dan Teknologi

Seluruh proyek ini dibangun dengan tools dan library berikut:

| Tools / Library   | Keterangan |
|-------------------|------------|
| Python            | Bahasa utama dalam analisis |
| Pandas            | Untuk manipulasi dan analisis data |
| scikit-learn      | Untuk clustering dan preprocessing |
| Matplotlib        | Visualisasi data dalam bentuk grafik |
| Seaborn           | Grafik statistik berbasis Matplotlib |
| Plotly (opsional) | Visualisasi interaktif dan 3D |
| Jupyter Notebook  | Platform interaktif untuk coding dan dokumentasi |
| Openpyxl          | Digunakan kalau data dalam format Excel (.xlsx) |
