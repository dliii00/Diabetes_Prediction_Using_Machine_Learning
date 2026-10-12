# Prediksi Diabetes Menggunakan Machine Learning

## Deskripsi Proyek

Proyek ini bertujuan untuk melakukan prediksi diabetes menggunakan metode Machine Learning berdasarkan karakteristik kesehatan dan gaya hidup pasien.

Dataset yang digunakan berisi informasi mengenai:

- Jenis kelamin
- Usia
- Hipertensi
- Penyakit jantung
- Riwayat merokok
- BMI (Body Mass Index)
- HbA1c
- Kadar glukosa darah
- Status diabetes

Variabel target yang digunakan adalah `diabetes`, dengan nilai:

- `0` = Tidak diabetes
- `1` = Diabetes

---

## Dataset

Dataset berisi data pasien dengan beberapa karakteristik kesehatan dan gaya hidup.

### Variabel Dataset

| Variabel | Deskripsi |
|---|---|
| `gender` | Jenis kelamin pasien |
| `age` | Usia pasien |
| `hypertension` | Status hipertensi |
| `heart_disease` | Status penyakit jantung |
| `smoking_history` | Riwayat merokok |
| `bmi` | Body Mass Index |
| `HbA1c_level` | Tingkat HbA1c |
| `blood_glucose_level` | Kadar glukosa darah |
| `diabetes` | Status diabetes sebagai variabel target |

---

## Exploratory Data Analysis

Tahapan Exploratory Data Analysis (EDA) yang dilakukan meliputi:

- Melihat struktur dataset
- Memeriksa tipe data
- Statistik deskriptif
- Memeriksa missing value
- Mengidentifikasi variabel numerik dan kategorikal
- Visualisasi distribusi data
- Membuat box plot
- Mendeteksi outlier menggunakan metode IQR
- Melihat distribusi variabel target
- Analisis korelasi antarvariabel

Tahapan ini dilakukan untuk memahami karakteristik dataset sebelum digunakan dalam proses Machine Learning.

---

## Preprocessing Data

Tahapan preprocessing yang dilakukan meliputi:

1. Memeriksa tipe data
2. Memeriksa missing value
3. Mengidentifikasi fitur numerik dan kategorikal
4. Mendeteksi outlier
5. Melakukan encoding pada data kategorikal
6. Melakukan standardisasi pada fitur numerik
7. Membagi dataset menjadi data training dan testing

Variabel kategorikal seperti `gender` dan `smoking_history` diproses menggunakan encoding agar dapat digunakan oleh algoritma Machine Learning.

Fitur numerik seperti:

- `age`
- `bmi`
- `HbA1c_level`
- `blood_glucose_level`

diproses menggunakan standardisasi sesuai kebutuhan model.

---

## Machine Learning

Permasalahan pada proyek ini merupakan **binary classification**, karena variabel target `diabetes` hanya memiliki dua kelas:

```text
0 = Tidak Diabetes
1 = Diabetes
