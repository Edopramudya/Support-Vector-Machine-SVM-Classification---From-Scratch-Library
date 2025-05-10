# Support Vector Machine (SVM) Classification - From Scratch & Library
Repositori ini berisi implementasi algoritma **Support Vector Machine (SVM)** untuk klasifikasi data sederhana (berbasis berat dan tinggi badan) ke dalam dua kelas: *soccer* dan *sumo*. Proyek ini mencakup pendekatan **manual (from scratch)** dan juga pendekatan menggunakan **library Scikit-learn**, lengkap dengan visualisasi hyperplane dan margin.

## 🔍 Deskripsi Proyek
Tujuan dari proyek ini adalah untuk mempelajari dan memvisualisasikan bagaimana SVM bekerja, baik secara konseptual (manual) maupun praktis (library). Model digunakan untuk memisahkan dua kelas berdasarkan dua fitur input: **Weight (Berat)** dan **Height (Tinggi Badan)**.

## 📌 Isi Notebook
Notebook ini dibagi menjadi 3 bagian utama:
1. **SVM From Scratch (Dua Sampel Saja)**
   Membangun SVM secara manual hanya dengan dua data perwakilan dari masing-masing kelas. Digunakan untuk menyusun sistem persamaan dan mencari parameter $w_1$, $w_2$, dan $b$ secara langsung.
2. **SVM From Scratch (Semua Data / Grid Search)**
   Implementasi pencarian parameter optimal $w$ dan $b$ menggunakan **brute-force** (grid search). Diperiksa seluruh data untuk memastikan semua memenuhi constraint margin $y(w \cdot x + b) \geq 1$, lalu dipilih parameter dengan margin terkecil.
3. **SVM dengan Scikit-learn**
   Menggunakan `SVC(kernel='linear')` dari Scikit-learn untuk klasifikasi data dan membandingkan hasilnya dengan implementasi manual. Disertai visualisasi garis pemisah (hyperplane), margin, dan support vector.

## 📊 Visualisasi
Untuk setiap pendekatan, notebook menyajikan:
* Scatter plot dari data asli
* Garis hyperplane (f(x) = 0)
* Margin atas (+1) dan bawah (−1)

## 📁 Dataset
Dataset kecil berisi 6 entri:

| Weight | Height | Label  |
| ------ | ------ | ------ |
| 67     | 167    | soccer |
| 68     | 169    | soccer |
| 71     | 175    | soccer |
| 142    | 191    | sumo   |
| 135    | 186    | sumo   |
| 130    | 182    | sumo   |

Label dikonversi ke **+1 untuk soccer** dan **−1 untuk sumo**.

## ⚙️ Tools
* Python (NumPy, Matplotlib)
* Scikit-learn
* Jupyter Notebook

## 🧠 Tujuan Pembelajaran
* Memahami konsep dasar margin, hyperplane, dan constraint SVM
* Menerapkan teori SVM ke dalam kode Python
* Membandingkan pendekatan manual dengan pendekatan library

