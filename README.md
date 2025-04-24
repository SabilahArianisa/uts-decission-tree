
# Decision Tree Classifier untuk Dataset dari Google Drive

## Deskripsi Proyek

Proyek ini menggunakan algoritma **Decision Tree Classifier** dari Scikit-learn untuk melakukan klasifikasi berdasarkan dataset yang disimpan di Google Drive. Model ini dilatih dan dievaluasi dengan membagi data ke dalam data latih dan data uji.

## Langkah-langkah

1. **Import Library**  
   Mengimpor library yang dibutuhkan seperti `pandas`, `scikit-learn` untuk preprocessing data, pelatihan model, dan evaluasi.

2. **Baca Dataset dari Google Drive**  
   Dataset diakses langsung melalui tautan berbentuk file ID dari Google Drive, kemudian dibaca menggunakan `pandas.read_csv()`.

3. **Tampilkan Contoh Data**  
   Menampilkan beberapa baris pertama dari dataset untuk memahami struktur dan isi datanya.

4. **Pra-pemrosesan (One-hot Encoding)**  
   Melakukan encoding terhadap data kategorikal menggunakan metode one-hot encoding, menghindari dummy trap dengan `drop_first=True`.

5. **Deteksi Kolom Target Secara Otomatis**  
   Mendeteksi kolom target berdasarkan nama kolom yang mengandung kata kunci seperti 'BUY' atau 'COMPUTER'.

6. **Pisahkan Fitur dan Label**  
   Data dipisahkan antara fitur (independen) dan label (dependen) berdasarkan kolom target yang terdeteksi.

7. **Split Dataset**  
   Membagi data menjadi data latih (training) dan data uji (testing) dengan perbandingan 80:20.

8. **Latih Model Decision Tree**  
   Model Decision Tree dilatih menggunakan data latih. Parameter `random_state` digunakan agar hasil replikasi tetap konsisten.

9. **Evaluasi Model**  
   Model diuji dengan data uji, dan hasilnya dianalisis menggunakan confusion matrix, classification report, dan akurasi.

---

Kalau kamu perlu tambahan untuk cara menjalankan, dependencies, atau contoh output, tinggal bilang ya!
