# 🧠 Mental Health Condition Classification

## 📌 Deskripsi
Project ini bertujuan untuk melakukan **klasifikasi kondisi kesehatan mental** responden berdasarkan data gaya hidup, kebiasaan, serta faktor sosial dan psikologis. Kondisi yang diprediksi mencakup beberapa kategori, seperti:
- Anxiety
- Depression
- Bipolar
- PTSD

Dengan memanfaatkan algoritma *machine learning* seperti **Support Vector Machine (SVM)**, **Random Forest**, dan **Logistic Regression**, project ini berupaya membandingkan performa model dalam mengidentifikasi pola yang berhubungan dengan kesehatan mental.

---

## 📂 Dataset
### 🌐 Sumber Data
Dataset diperoleh dari sumber terbuka mengenai survei kesehatan mental. Data ini berisi informasi responden dari berbagai negara dengan latar belakang demografis berbeda.

### 📊 Keterangan Data
Beberapa variabel utama yang digunakan:
- **Sleep Hours** → Jam tidur per hari responden  
- **Screen Time per Day (Hours)** → Durasi penggunaan layar dalam sehari  
- **Social Interaction Score** → Tingkat interaksi sosial responden  
- **Happiness Score** → Skor kebahagiaan  
- **Work Hours per Week** → Jam kerja per minggu  
- **Mental Health Condition** → Label target (Anxiety, Depression, Bipolar, PTSD)

---

## 🧹 Tahapan Analisis
1. **Definisi Library** 📚  
   Mengimpor library Python yang dibutuhkan seperti pandas, numpy, matplotlib, seaborn, dan scikit-learn.  

2. **Baca Dataset** 📂  
   Membaca data mentah, memahami struktur, serta memeriksa isi dataset.  

3. **Pembersihan Data** 🧹  
   - ⭕ **Cek Nilai Kosong** → Identifikasi missing values  
   - 🗑️ **Penghapusan Data** → Menghapus data yang tidak relevan atau rusak  

4. **EDA (Exploratory Data Analysis)** 🔎  
   Analisis eksploratif untuk memahami pola data, seperti:  
   - Distribusi responden per negara 🌍  
   - Distribusi responden per jenis kelamin 🚻  
   - Distribusi kondisi kesehatan mental 🧠  
   - Hubungan kondisi kesehatan mental dengan negara & jenis kelamin  

5. **Correlation Matrix** 🔢  
   Visualisasi matriks korelasi untuk melihat hubungan antar variabel numerik.  

6. **Data Mining** ⛏️  
   Melakukan kategorisasi variabel (Sleep Category, Screen Time Category, dll.) serta encoding variabel kategorikal menjadi numerik.  

7. **Implementasi Model** 🤖  
   Menerapkan tiga algoritma utama:  
   - 🧩 **Support Vector Machine (SVM)**  
   - 🌳 **Random Forest**  
   - 📉 **Logistic Regression**  

---

## 📈 Hasil
Hasil evaluasi model ditampilkan dalam bentuk **confusion matrix** dan **classification report**.  
- **SVM** → Akurasi 28% (cukup baik mengenali PTSD)  
- **Random Forest** → Akurasi 24% (lebih baik pada Depression, tapi cenderung overfitting)  
- **Logistic Regression** → Akurasi 24% (cukup baik mengenali Anxiety, tapi lemah di Depression)  

Meskipun akurasi masih rendah, hasil ini menunjukkan bagaimana faktor-faktor gaya hidup dapat digunakan untuk analisis kesehatan mental menggunakan machine learning.  

---
