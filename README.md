# Analisis & Prediksi Data COVID-19 di Indonesia

Proyek ini berfokus pada proses pembersihan data (*data cleaning*), eksplorasi dan visualisasi tren deret waktu (*time series*), serta pemodelan prediksi kasus COVID-19 di Indonesia menggunakan Python di Google Colab.

## Fitur Utama
* **Data Cleaning & Preprocessing:** Memfilter data skala nasional (`Indonesia`), mengonversi kolom tanggal ke format `datetime`, mengurutkan data secara kronologis, serta menangani *missing values*.
* **Visualisasi Tren:** Memvisualisasikan kasus baru harian dan *moving average* 7 hari untuk melihat pola gelombang kasus.
* **Pemodelan Prediksi (*Forecasting*):** Menggunakan fitur *lag* dengan model regresi (seperti `RandomForestRegressor`) dan/atau model deret waktu (`Prophet`) untuk memprediksi tren ke depan serta mengevaluasinya dengan metrik MAE dan RMSE.

## Struktur Proyek
* `notebook.ipynb` — Notebook utama berisi alur pembersihan data, visualisasi, dan pemodelan prediksi di Google Colab.
* `README.md` — Dokumentasi proyek.

## Teknologi & Pustaka
* Python 3
* `pandas` & `numpy`
* `matplotlib`
* `scikit-learn`
* `seaborn`

## Cara Menjalankan
1. Buka notebook di **Google Colab** atau lingkungan Jupyter/Python lokal Anda.
2. Muat dataset COVID-19 Indonesia (misalnya dari Kaggle) ke dalam *DataFrame* `df`.
3. Jalankan sel secara berurutan mulai dari pembersihan data, visualisasi, hingga pelatihan dan evaluasi model.

## Evaluasi & Catatan
* Pembagian data latih dan uji dilakukan secara kronologis agar tidak terjadi kebocoran informasi masa depan (*data leakage*).
* Hasil prediksi sangat bergantung pada kualitas data historis dan perubahan pola pelaporan maupun dinamika kasus di lapangan.
