# Prediksi Penyakit Jantung Menggunakan Deep Learning (Artificial Neural Network)

## Identitas Kelompok
- Nama Anggota 1 : Nathanael Lesmana
- Nama Anggota 2 : Fahmi Imam Taufik
- Nama Anggota 3 : Ariya Maulana Arifin
- Nama Anggota 4 : ..................................
- Nama Anggota 5 : ..................................

Program Studi : Teknik Informatika  
Mata Kuliah    : Deep Learning  
Semester       : 7 A 
Dosen Pengampu : Asriyanik, M.T.

---

## Latar Belakang dan Tujuan
Penyakit jantung merupakan salah satu penyebab utama kematian di dunia. Deteksi dini
penyakit jantung sangat penting untuk membantu proses pengambilan keputusan medis.
Dengan berkembangnya teknologi kecerdasan buatan, khususnya Deep Learning,
prediksi penyakit dapat dilakukan secara otomatis berdasarkan data medis pasien.

Tujuan dari proyek ini adalah membangun model Deep Learning berbasis
**Artificial Neural Network (ANN)** untuk memprediksi apakah seseorang
mengidap penyakit jantung atau tidak berdasarkan data klinis.

---

## Deskripsi Dataset
Dataset yang digunakan pada penelitian ini adalah **Heart Disease Dataset**
yang berasal dari UCI Machine Learning Repository dan tersedia secara publik
melalui platform Kaggle.

Karakteristik dataset:
- Jumlah data: 303 sampel
- Jumlah fitur: 13 fitur input
- 1 label target (binary classification)
- Tipe data: Tabular

Target:
- 0 : Tidak mengidap penyakit jantung
- 1 : Mengidap penyakit jantung

Sumber dataset:
Kaggle – Heart Disease UCI Dataset

---

## Pra-pemrosesan Data
Tahapan pra-pemrosesan data yang dilakukan meliputi:
1. Data cleaning dan pengecekan nilai kosong
2. Pemisahan fitur dan label
3. Normalisasi data menggunakan StandardScaler
4. Pembagian data menjadi:
   - Data training (70%)
   - Data validation (15%)
   - Data testing (15%)

Tahapan ini bertujuan untuk meningkatkan performa model dan
memastikan data berada pada skala yang seragam.

---

## Metodologi dan Arsitektur Model
Model yang digunakan pada proyek ini adalah **Artificial Neural Network (ANN)**
yang termasuk dalam kategori Deep Learning.

Arsitektur model:
- Input layer: 13 neuron
- Hidden layer 1: 64 neuron (ReLU)
- Hidden layer 2: 32 neuron (ReLU)
- Output layer: 1 neuron (Sigmoid)

Konfigurasi pelatihan:
- Loss function: Binary Crossentropy
- Optimizer: Adam
- Epoch: 50
- Batch size: 16

Model dilatih menggunakan data training dan divalidasi menggunakan data validation.

---

## Hasil dan Evaluasi
Evaluasi model dilakukan menggunakan data testing dengan metrik:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Grafik loss training dan validation

Hasil evaluasi menunjukkan bahwa model mampu mencapai akurasi yang baik
dalam memprediksi penyakit jantung, dengan perbedaan loss training dan validation
yang relatif kecil.

---

## Analisis dan Pembahasan
Berdasarkan hasil pelatihan dan evaluasi, model ANN mampu mempelajari
pola dari data tabular dengan cukup baik.
Tidak terdapat indikasi overfitting yang signifikan,
karena nilai loss pada data training dan validation menunjukkan tren yang stabil.

Kelebihan model:
- Arsitektur sederhana dan mudah dipahami
- Performa cukup baik untuk dataset tabular
- Waktu pelatihan relatif cepat

Keterbatasan model:
- Jumlah dataset relatif kecil
- Model belum diuji pada data nyata di luar dataset

---

## Kesimpulan
Pada proyek ini telah berhasil dibangun model Deep Learning berbasis
Artificial Neural Network untuk memprediksi penyakit jantung.
Model menunjukkan performa yang baik dan dapat digunakan sebagai
sistem pendukung keputusan awal dalam bidang kesehatan.

Pengembangan lebih lanjut dapat dilakukan dengan menambahkan jumlah data,
melakukan tuning hyperparameter, atau membandingkan dengan arsitektur
Deep Learning lainnya.

---

## Referensi
1. UCI Machine Learning Repository – Heart Disease Dataset  
2. Kaggle – Heart Disease UCI Dataset  
3. Goodfellow, I., Bengio, Y., & Courville, A. (2016). Deep Learning. MIT Press  
4. Dokumentasi TensorFlow & Keras
