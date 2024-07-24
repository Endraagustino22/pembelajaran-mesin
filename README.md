# pembelajaran-mesin
praktikum pembelajaran mesin

## ringkasan : 
project prediksiHargaRumah ini bertujuan untuk memprediksi Harga rumah di jaksel berdasarkan dataset yang di ambil dari kagle menggunakan supervised learning yaitu model XGBRegressor, karena belum ada yang menggunakan model tersebut di kaggle tersebut.


## permasalahan : 
memprediksi Harga rumah(label) berdasarkan feature-feature dari dataset, seperti luas tanah, luas bangunan, jumlah kamar tidur, jumlah kamar mandi, dan keberadaan garasi agar bisa membuat machine learning dengan akurasi yang baik

## tujuan :  
untuk memprediksi Harga rumah di jaksel berdasarkan feature-feature yang tersedia di dataset. dan mengoptimalkan model untuk mendapatkan performa terbaik dalam hal akurasi dan matriks evaluasi lainnya

## Model :
menggunakan model XGBoost Regressor (XGBRegressor), yaitu model yang menggunakan teknik boosting untuk membangun model prediksi dengan menggabungkan beberapa pohon keputusan (decision trees) secara bertahap. Setiap pohon keputusan yang baru dibangun berusaha memperbaiki kesalahan dari pohon keputusan sebelumnya.

## bagan :
![diagram_ML_hargaRumah drawio (1)](https://github.com/user-attachments/assets/5669a91f-c836-4034-bd60-3cea9992383e)


## Penjelasan dataset :
Dataset harga rumah jaksel terdiri dari 7 kolom dengan jumlah data yaitu 1000 data. Kolom tersebut terdiri dari :
 - HARGA : harga dari rumah.
 - LT : jumlah luas tanah.
 - LB : jumlah luas bangunan.
 - JKT : jumlah kamar tidur.
 - JKM : jumlah kamar mandi.
 - GRS : ada/tidak ada
 - KOTA : nama kota.
 source (https://www.kaggle.com/datasets/wisnuanggara/daftar-harga-rumah)
 
## EDA :
![Screenshot 2024-07-25 025517](https://github.com/user-attachments/assets/1b093581-cca6-4717-8e30-866401c203bd)


![Screenshot 2024-07-25 033250](https://github.com/user-attachments/assets/598ecbd5-6ca8-4099-af30-9af00b0eb958)

 
## proses learning modeling : 
XGBRegressor merupakan sebuah model regresi yang menggunakan teknik gradient boosting. Meskipun berbasis pada decision tree, XGBRegressor tidak hanya berupa satu decision tree, tetapi merupakan kumpulan dari banyak decision tree yang dioptimalkan melalui proses boosting.

Secara spesifik, XGBRegressor adalah implementasi dari algoritma XGBoost, yang bekerja dengan cara membangun banyak decision tree secara iteratif. Setiap tree baru dibangun untuk memperbaiki kesalahan dari tree sebelumnya. Proses ini membantu meningkatkan akurasi model secara keseluruhan.

Jadi, XGBRegressor adalah decision tree yang digunakan dalam konteks boosting, dan lebih tepatnya, ia menggunakan teknik gradient boosting untuk menggabungkan banyak decision tree dalam satu model yang kuat.


## performa model :
hasil model
 - train score (r-squared-score)= 0.7315719538442023
 - test score (r-squred-score)= 0.6402377268428613
 - RMSE: 8.53467752861412
 - MSE = 72.84072051743081
 - MAE = 5.045983975064103
 
## kesimpulan : 
 hasil dari model machine learning XGBRegressor untuk memprediksi harga rumah di jaksel masih kurang baik. beberapa alasanya yaitu : kurang banyaknya feature-feature untuk memprediksi label agar lebih akurat dan butuh lebih banyak lagi data agar model bisa lebih akurat. 
