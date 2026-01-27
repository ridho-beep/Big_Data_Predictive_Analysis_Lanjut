\# 🛒 Analisis dan Prediksi Perilaku Pembelian Pengguna E-Commerce  

\### Menggunakan PySpark dan Machine Learning Berbasis Big Data



---



\## 📌 Deskripsi Proyek

Proyek ini bertujuan untuk menganalisis perilaku pengguna pada platform e-commerce dan membangun model machine learning untuk memprediksi apakah pengguna yang telah memasukkan produk ke keranjang (\*cart\*) akan melakukan pembelian (\*purchase\*).  

Pemrosesan data dilakukan menggunakan \*\*PySpark\*\* untuk menangani data berskala besar (Big Data), serta algoritma \*\*Logistic Regression\*\* dan \*\*Random Forest\*\* untuk melakukan klasifikasi.



---



\## 📂 Dataset

Dataset yang digunakan merupakan data aktivitas pengguna e-commerce periode \*\*Oktober 2019\*\*, yang berisi jutaan catatan interaksi pengguna.



\### Atribut Dataset:

| Kolom        | Deskripsi |

|--------------|-----------|

| `event\_type` | Jenis aktivitas pengguna (\*view, cart, purchase\*) |

| `product\_id` | ID unik produk |

| `category\_id`| ID kategori produk |

| `price`      | Harga produk |

| `user\_id`    | ID pengguna |



Dataset berskala besar sehingga dilakukan \*\*sampling data\*\* untuk efisiensi komputasi.



---



\## 🧩 Alur Pengerjaan (Pipeline Big Data)



1\. \*\*Load Data\*\*  

&nbsp;  Membaca dataset CSV menggunakan PySpark



2\. \*\*Data Cleaning \& Preprocessing\*\*  

&nbsp;  - Menghapus missing value  

&nbsp;  - Validasi nilai harga  

&nbsp;  - Casting tipe data  



3\. \*\*Exploratory Data Analysis (EDA)\*\*  

&nbsp;  - Distribusi event\_type  

&nbsp;  - Statistik harga produk  

&nbsp;  - MapReduce menggunakan RDD  



4\. \*\*Pembuatan Label (Supervised Learning)\*\*  

&nbsp;  - Label `1`: User cart → purchase  

&nbsp;  - Label `0`: User cart → tidak purchase  



5\. \*\*Feature Engineering\*\*  

&nbsp;  - VectorAssembler untuk membentuk fitur numerik  



6\. \*\*Pemodelan Machine Learning\*\*  

&nbsp;  - Logistic Regression  

&nbsp;  - Random Forest  



7\. \*\*Evaluasi \& Komparasi Model\*\*  

&nbsp;  - F1-Score  

&nbsp;  - Confusion Matrix  

&nbsp;  - Accuracy, Precision, Recall  



8\. \*\*Hyperparameter Tuning\*\*  

&nbsp;  - Peningkatan performa model terbaik  



---



\## 🤖 Model yang Digunakan



| Model | Keterangan |

|------|------------|

| Logistic Regression | Baseline model |

| Random Forest | Model utama dengan performa terbaik |



\### 🔥 Hasil Akhir (After Tuning)

\- \*\*F1-Score:\*\* \*\*89.05%\*\*

\- Model terbaik: \*\*Random Forest\*\*



---



\## 📊 Evaluasi Model



Evaluasi dilakukan menggunakan:

\- Multiclass Classification Evaluator

\- Confusion Matrix



\### Confusion Matrix (Random Forest After Tuning)

Model menunjukkan performa sangat baik dalam mengklasifikasikan pengguna yang tidak membeli, serta stabil dalam mendeteksi pembelian meskipun data tidak seimbang.



---



\## 🧠 Kesimpulan

\- PySpark efektif untuk memproses Big Data e-commerce

\- Random Forest memberikan performa terbaik dalam memprediksi pembelian

\- Model dapat dimanfaatkan untuk:

&nbsp; - Sistem rekomendasi

&nbsp; - Retargeting promosi

&nbsp; - Analisis perilaku pelanggan



---



\## 🛠️ Teknologi yang Digunakan

\- Python

\- PySpark

\- Apache Spark MLlib

\- Google Colab

\- Matplotlib



---

