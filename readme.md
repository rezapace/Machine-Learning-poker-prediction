# Poker Prediction

# HOW TO RUN PROJECT

1. Download the Jupyter notebook:
   ```bash
   wget https://github.com/rezapace/Machine-Learning-poker-prediction/releases/download/1.0/poker_prediction.ipynb
   ```

2. Open Google Colab:
   [https://colab.research.google.com/#create=true](https://colab.research.google.com/#create=true)

3. Upload the downloaded `klasifikasi_catur.ipynb` file to Google Colab.

4. Run the notebook:
   - Execute each cell in order
   - Follow the instructions provided in the notebook comments

Note: Make sure you have a Google account to use Google Colab. If you encounter any issues, please refer to the [project repository](https://github.com/rezapace/Machine-Learning-poker-prediction) for troubleshooting or to report problems.

## Deskripsi
Proyek ini bertujuan untuk membuat model prediksi kemenangan dalam permainan poker menggunakan dataset yang dihasilkan secara acak. Model ini menggunakan algoritma Random Forest untuk memprediksi probabilitas kemenangan berdasarkan berbagai fitur seperti kartu hole, posisi pemain, jumlah pemain yang tersisa, ukuran pot, dan jumlah taruhan yang harus dipanggil.

## Kegunaan
Proyek ini berguna untuk:
1. Mempelajari cara menghasilkan dataset poker secara acak.
2. Menerapkan teknik preprocessing data untuk mempersiapkan dataset.
3. Melatih model prediksi menggunakan algoritma Random Forest.
4. Mengevaluasi performa model prediksi.
5. Memprediksi probabilitas kemenangan berdasarkan input kartu dan kondisi permainan.

## Fungsi
Proyek ini terdiri dari beberapa fungsi utama:
1. `generate_all_cards()`: Menghasilkan semua kombinasi kartu yang mungkin.
2. `hand_strength(card1, card2)`: Menghitung kekuatan tangan berdasarkan dua kartu.
3. `generate_poker_dataset(n_samples)`: Menghasilkan dataset poker dengan jumlah sampel yang ditentukan.
4. `card_to_value(card)`: Mengonversi kartu menjadi nilai numerik.
5. `predict_win_probability(card1, card2, position, players_left, pot_size, bet_to_call)`: Memprediksi probabilitas kemenangan berdasarkan input kartu dan kondisi permainan.

## Bagaimana Menjalankan
1. **Persiapan Lingkungan**:
   - Pastikan Anda memiliki Python dan Jupyter Notebook terinstal di sistem Anda.
   - Instal pustaka yang diperlukan dengan menjalankan perintah berikut:
     ```bash
     pip install pandas numpy scikit-learn matplotlib seaborn
     ```

2. **Menjalankan Notebook**:
   - Buka Jupyter Notebook dan muat file `poker_prediction.ipynb`.
   - Jalankan setiap sel dalam notebook untuk menghasilkan dataset, melatih model, dan melakukan prediksi.

3. **Menghasilkan Dataset**:
   - Tentukan jumlah sampel yang diinginkan dengan mengubah nilai `n_samples` pada sel yang sesuai.
   - Jalankan sel untuk menghasilkan dataset dan menyimpannya dalam file CSV.

4. **Melatih Model**:
   - Jalankan sel yang memuat dataset, melakukan preprocessing, dan melatih model Random Forest.

5. **Memprediksi Kemenangan**:
   - Gunakan fungsi `predict_win_probability` dengan memasukkan kartu dan kondisi permainan untuk memprediksi probabilitas kemenangan.

## Kesimpulan
Proyek ini menunjukkan bagaimana kita dapat menggunakan teknik pembelajaran mesin untuk memprediksi probabilitas kemenangan dalam permainan poker. Dengan menghasilkan dataset secara acak dan melatih model prediksi, kita dapat memahami faktor-faktor yang mempengaruhi kemenangan dalam poker. Model Random Forest yang digunakan dalam proyek ini memberikan akurasi yang baik dan dapat digunakan untuk memprediksi hasil permainan berdasarkan input yang diberikan.