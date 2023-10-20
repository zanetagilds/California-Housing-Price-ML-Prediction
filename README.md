# California Housing Price Machine Learning Prediction

## Context
California, Amerika Serikat merupakan destinasi idaman untuk dihuni. Kota-kota terkenal seperti Los Angeles, San Francisco, dan San Diego menjadi daya tarik utama. Cuaca yang cenderung hangat sepanjang tahun, keberagaman pantai yang memukau menjadi daya tarik tersendiri bagi masyarakat yang ingin menetap di sini. Menurut [Forbes Home](https://www.forbes.com/home-improvement/features/states-with-highest-home-prices/), California menempati peringkat kedua sebagai negara bagian termahal untuk memiliki properti, mulai dari harga rumah dan pajaknya. Terlepas dari itu, terdapat banyak peminat yang ingin menghuni di California. Pada dataset ini, tersedia informasi mengenai harga rumah di California pada tahun 1990, yang berasal dari data sensus pada tahun tersebut. Dataset ini terdokumentasi dalam karya ilmiah yang berjudul "Sparse Spatial Autoregressions" oleh R. Kelley Pace dan Ronald Barry. Dataset mencakup beragam informasi, seperti populasi, pendapatan median, median harga rumah, jumlah total kamar tidur, dan informasi lainnya. 

## Problem Statement
Sebagai **real estate developer**, **memprediksi harga rumah yang akurat dan dalam waktu yang singkat sangat krusial dalam bisnis mereka**. Hal tersebut berguna agar rumah yang dibangun cepat terjual dan tidak mengalami kerugian. **Prediksi melalui analisis harga pasar secara konvensional terkadang menghasilkan output yang tidak akurat** akibat subjektifitas para peneliti pada real estate developer dan juga **memakan waktu yang cenderung lama**. Untuk mengatasi masalah tersebut, **model machine learning** mampu menjawab atas permasalahan tersebut. **Oleh karena itu, diperlukan model machine learning untuk memberi harga prediksi rumah secara akurat dan waktu yang singkat**. 

## Analytical Approach
Analisis dilakukan dengan menggunakan semua fitur-fitur dari dataset. Langkah selanjutnya adalah **menggunakan model regresi untuk memprediksi harga rumah**. Model ini akan dijadikan sebuah pertimbangan bagi real estate developer dalam memprediksi harga rumah yang akurat dalam waktu yang singkat.

## Metrics Evaluation
Penggunaan **metrics evaluation pada pemodelan ini**, adalah sebagai berikut:
1. **RMSE (Root Mean Square Error)**: memprediksi nilai aktual dengan mengukur rata-rata akar dari selisih kuadrat antara nilai prediksi dan nilai aktual.Semakin rendah nilainya, tingkat akurasi semakin tinggi.
2. **MAE (Mean Absolute Error)**:  mengukur rata-rata kesalahan absolut antara nilai prediksi dan nilai aktual. Ini memberikan indikasi sejauh mana prediksi model dari nilai aktual dalam skala yang sama. MAE lebih tahan terhadap outlier dibandingkan RMSE.
3. **MAPE (Mean Absolute Percentage Error)**: mengukur rata-rata kesalahan persentase antara nilai prediksi dan nilai aktual. Ini memberikan pemahaman tentang sejauh mana prediksi model dari nilai aktual dalam bentuk persentase. MAPE berguna ketika perbandingan persentase kesalahan diperlukan.

## Goals
Berdasarkan permasalahan tersebut, goals dalam pemodelan California Housing Price adalah:
1. Memprediksi harga rumah yang akurat
2. Prediksi dilakukan dalam waktu yang cenderung sebentar

## Conclusion and Impact of the Model on Business
1. **Dari segi biaya dan waktu**
    Untuk memprediksi harga rumah, penelitian real estate developer membutuhkan waktu 8 minggu, tetapi dengan machine learning membutuhkan waktu 1 hingga 3 hari. Biaya penelitian real estate developer adalah $100 sehingga totalnya adalah $5.600, sedangkan maksimal biaya dengan machine learning adalah $300. Dengan menggunakan machine learning, anggaran dapat  dihemat dan waktu pelaksanaan menjadi lebih singkat.
2. **Dari segi actual dan predicted price**
    Nilai error sebanyak 17.5338% dengan rata-rata harga rumah dari kolom median_house_value adalah $206.824. Perhitungannya adalah sebagai berikut:
    17.5338% dari $206.824 adalah $36.17.

Oleh karena itu, berikut merupakan harga prediksi rumah apabila terjadi overestimation dan underestimation
- Harga prediksi yang overestimate: $206.824 + $36.17 =  $204.207
- Harga prediksi yang underestimate: $206.824 - $36.17 =  $210.441


## Rekomendasi
1. **Pemanfaatkan Model Machine Learning**: disarankan untuk mengimplementasikan model machine learning dalam proses prediksi harga rumah. Model ini dapat memberikan prediksi yang lebih akurat dan efisien daripada metode konvensional. Selain itu, lakukan validasi model secara berkala untuk memastikan bahwa model machine learning tetap akurat seiring berjalannya waktu. Hal ini penting karena pasar real estate cenderung berubah seiring berjalannya waktu.

2. **Optimisasi Waktu**: Manfaatkan model machine learning untuk menghasilkan prediksi dalam waktu yang lebih singkat. Dengan demikian, real estate developer mampu memprediksi harga dengan waktu yang cenderung singkat dibandingkan metode konvensional.

3. **Libatkan Data Scientist**: Meskipun model machine learning dapat memberikan prediksi yang akurat, peran data scientist dalam industri real estate tetap penting. Mereka dapat mengoptimalkan machine learning dengan data yang telah tersedia dari real estate developer.
