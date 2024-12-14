# Proyek Analisis Data: Kampanye Pemasaran

Proyek ini bertujuan untuk melakukan analisis data pada dataset kampanye pemasaran, melakukan clustering untuk segmentasi pelanggan, dan membangun model klasifikasi untuk memprediksi segmen pelanggan berdasarkan fitur-fitur tertentu.

## Struktur Proyek

Proyek ini terdiri dari beberapa file dan direktori sebagai berikut:

- `marketing_campaign.csv`: Dataset asli yang berisi informasi tentang pelanggan, termasuk demografi, perilaku belanja, dan interaksi produk.
- `marketing_campaign_with_clusters.csv`: Dataset hasil clustering yang berisi informasi tambahan tentang segmen pelanggan.
- `[Clustering]_Submission_Akhir_BMLP_Yoga_Rizki_Pratama.ipynb`: Notebook Jupyter yang berisi langkah-langkah analisis data dan clustering.
- `[Klasifikasi]_Submission_Akhir_BMLP_Yoga_Rizki_Pratama.ipynb`: Notebook Jupyter yang berisi langkah-langkah klasifikasi.

## Langkah-langkah Analisis

### 1. Import Library
Mengimpor pustaka Python yang dibutuhkan untuk analisis data dan pembangunan model machine learning. Pustaka yang digunakan: `pandas`, `numpy`, `sklearn`, `seaborn`, `matplotlib`, `lightgbm`.

### 2. Memuat Dataset
Memuat dataset asli (`marketing_campaign.csv`) dan dataset hasil clustering (`marketing_campaign_with_clusters.csv`) ke dalam variabel DataFrame. Menampilkan beberapa baris awal dataset untuk memahami strukturnya.

### 3. Data Splitting
Memisahkan dataset menjadi dua bagian: data latih (training set) dan data uji (test set). Melakukan one-hot encoding untuk kolom kategorikal.

### 4. Membangun Model Klasifikasi
Menggunakan algoritma LightGBM (Light Gradient Boosting Machine) untuk membangun model klasifikasi. Melakukan pencarian hyperparameter terbaik menggunakan RandomizedSearchCV. Melatih model menggunakan data latih dan menampilkan hyperparameter terbaik yang ditemukan.

### 5. Evaluasi Model Klasifikasi
Melakukan prediksi menggunakan data uji. Menghitung metrik evaluasi seperti Accuracy dan F1-Score. Membuat confusion matrix untuk melihat detail prediksi benar dan salah. Menampilkan classification report untuk data testing.

### 6. Tuning Model Klasifikasi (Optional)
Menggunakan SelectKBest untuk feature selection. Melakukan pencarian hyperparameter terbaik dengan fitur yang dipilih. Menghitung ulang metrik evaluasi untuk melihat apakah ada peningkatan performa.

### 7. Analisis Hasil Evaluasi Model Klasifikasi
Membandingkan hasil evaluasi sebelum dan setelah tuning. Mengidentifikasi kelemahan model, seperti precision atau recall rendah untuk kelas tertentu. Memberikan rekomendasi tindakan lanjutan, seperti mengumpulkan data tambahan atau mencoba algoritma lain jika hasil belum memuaskan.

## Cara Menjalankan Proyek

1. Pastikan Anda memiliki Python dan Jupyter Notebook terinstal di sistem Anda.
2. Instal pustaka yang diperlukan dengan menjalankan perintah berikut:
   ```sh
   pip install pandas numpy scikit-learn seaborn matplotlib lightgbm
3. Buka Jupyter Notebook dan jalankan file [Clustering]_Submission_Akhir_BMLP_Yoga_Rizki_Pratama.ipynb dan [Klasifikasi]_Submission_Akhir_BMLP_Yoga_Rizki_Pratama.ipynb.
4. Ikuti langkah-langkah yang dijelaskan dalam notebook untuk melakukan analisis data, clustering, dan klasifikasi.

## Kontak
Jika Anda memiliki pertanyaan atau memerlukan bantuan lebih lanjut, silakan hubungi:

- Nama: Yoga Rizki Pratama
- Email: yogarizkipratama@gmail.com
- ID Dicoding: yorizpra