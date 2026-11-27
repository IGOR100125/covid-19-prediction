Analisis & Prediksi Data COVID-19 Indonesia

Proyek ini berisi eksplorasi data, visualisasi tren, dan pemodelan prediksi kasus COVID-19 di Indonesia menggunakan Python dan Google Colab.

Gambaran Umum (Overview)

Tujuan utama proyek ini adalah menganalisis pola perkembangan kasus COVID-19 di Indonesia secara historis serta membangun model forecasting untuk memperkirakan tren kasus ke depan berdasarkan data deret waktu (time series).

Dataset

Data bersumber dari dataset publik COVID-19 Indonesia (seperti dataset time series COVID-19 Indonesia di Kaggle) yang memuat informasi harian maupun kumulatif, antara lain:

Date: Tanggal pencatatan data

Location: Wilayah/lokasi (tingkat Nasional seperti Indonesia maupun tingkat Provinsi)

New Cases & Total Cases: Kasus positif harian dan kumulatif

New Deaths & Total Deaths: Kematian harian dan kumulatif

New Recovered & Total Recovered: Kesembuhan harian dan kumulatif

Alur Kerja (Workflow)

Pembersihan & Preparasi Data (Data Cleaning)

Memfilter data skala nasional (Location == 'Indonesia').

Mengonversi kolom Date ke format datetime dan mengurutkannya secara kronologis.

Memeriksa missing values serta memilih kolom utama yang relevan.

Analisis Eksploratif & Visualisasi

Memvisualisasikan tren kasus harian dan kumulatif.

Menggunakan 7-day moving average untuk menghaluskan fluktuasi harian dan melihat gelombang kasus secara lebih jelas.

Pemodelan Prediksi (Forecasting)

Pendekatan Machine Learning (misalnya Random Forest Regressor): Memanfaatkan fitur lag (kasus pada beberapa hari sebelumnya) dan membagi data secara kronologis menjadi data latih (train) dan data uji (test).

Pendekatan Time Series (misalnya Prophet): Memodelkan tren serta pola musiman mingguan/tahunan untuk proyeksi beberapa hari ke depan.

Evaluasi Model

Mengukur akurasi prediksi menggunakan metrik seperti MAE (Mean Absolute Error) dan RMSE (Root Mean Squared Error).

Cara Menjalankan di Google Colab

Buka file notebook (.ipynb) di Google Colab.

Unggah file dataset (.csv) ke lingkungan Colab atau hubungkan dengan Google Drive.

Jalankan setiap sel secara berurutan mulai dari import library, pembersihan data, visualisasi, hingga pelatihan dan evaluasi model.

(Opsional) Jika menggunakan library tambahan seperti prophet, jalankan instalasi terlebih dahulu (!pip install prophet).

Teknologi & Libraries

Python

Pandas & NumPy (manipulasi dan komputasi data)

Matplotlib / Seaborn (visualisasi data)

Scikit-learn (pemodelan machine learning & metrik evaluasi)

Prophet (pemodelan time series forecasting)

Catatan

Hasil prediksi sangat bergantung pada kualitas data historis, perubahan kebijakan kesehatan masyarakat, varian virus, serta dinamika pelaporan kasus di lapangan, sehingga sebaiknya digunakan sebagai bahan analisis eksploratif dan pembelajaran.
