# Laporan Proyek Machine Learning

### Nama : Arif Rahman Hakim

### Nim : 211351025

### Kelas : Pagi A

## Domain Proyek

Tujuan proyek ini adalah untuk menganalisis pola penjualan dan perilaku pelanggan dalam bisnis e-commerce berdasarkan dataset transaksi penjualan online yang diberikan. Dengan menganalisis data ini, kita dapat memahami tren penjualan, mengidentifikasi pelanggan berharga, melakukan segmentasi pelanggan, memprediksi penjualan di masa depan, dan melakukan analisis geografis terkait penjualan dan perilaku pelanggan.

## Business Understanding

Tujuan proyek ini adalah untuk menganalisis pola pembelian produk dalam bisnis e-commerce berdasarkan data transaksi penjualan online selama dua tahun. Hal ini bertujuan untuk memahami preferensi pelanggan, tren penjualan, dan faktor-faktor yang mempengaruhi kesuksesan bisnis

### Problem Statementsbard

- Masalah Utama: Bisnis e-commerce ini ingin memahami pola pembelian produk yang terjadi di platform mereka. Mereka ingin mengetahui kombinasi produk yang sering dibeli bersamaan oleh pelanggan, produk yang paling diminati, dan faktor-faktor yang mempengaruhi pembelian pelanggan. Dengan pemahaman ini, bisnis dapat mengoptimalkan strategi pemasaran, meningkatkan penjualan, dan meningkatkan kepuasan pelanggan.

- Tantangan Analisis: Tantangan utama dalam proyek ini adalah menganalisis data transaksi penjualan online yang besar dan kompleks. Data tersebut mencakup informasi tentang nomor faktur, kode produk, jumlah produk, tanggal transaksi, harga satuan, nomor pelanggan, dan negara pelanggan. Tantangan lainnya adalah mengidentifikasi pola pembelian yang relevan dan memberikan rekomendasi produk yang spesifik untuk meningkatkan penjualan.

### Goals

- Mengidentifikasi Pola Pembelian: Tujuan utama proyek ini adalah untuk mengidentifikasi pola pembelian produk dalam bisnis e-commerce berdasarkan data transaksi penjualan online selama dua tahun. Hal ini meliputi identifikasi kombinasi produk yang sering dibeli bersamaan oleh pelanggan, produk yang paling diminati, dan hubungan antara produk yang dibeli.
- Meningkatkan Strategi Pemasaran: Dengan pemahaman yang lebih baik tentang pola pembelian, tujuan proyek ini adalah untuk memberikan wawasan yang dapat membantu dalam mengoptimalkan strategi pemasaran. Hal ini dapat mencakup pengembangan kampanye promosi yang lebih efektif, pengelolaan persediaan yang lebih baik, dan penargetan pelanggan yang lebih tepat.
- Meningkatkan Penjualan: Salah satu tujuan utama proyek ini adalah untuk meningkatkan penjualan bisnis e-commerce. Dengan menganalisis pola pembelian, dapat diidentifikasi peluang untuk meningkatkan penjualan dengan menawarkan produk yang saling terkait atau memberikan rekomendasi produk yang relevan kepada pelanggan.
- Meningkatkan Kepuasan Pelanggan: Dengan memahami preferensi pelanggan dan memberikan rekomendasi produk yang relevan, tujuan proyek ini adalah untuk meningkatkan kepuasan pelanggan. Hal ini dapat mencakup memberikan pengalaman belanja yang personal, meningkatkan retensi pelanggan, dan membangun hubungan jangka panjang dengan pelanggan.

  ### Solution statements

- Analisis Pola Pembelian: Solusi untuk proyek ini adalah melakukan analisis mendalam terhadap data transaksi penjualan online untuk mengidentifikasi pola pembelian yang terjadi. Melalui teknik analisis seperti association rule mining atau market basket analysis, dapat diidentifikasi kombinasi produk yang sering dibeli bersamaan oleh pelanggan, produk yang paling diminati, dan hubungan antara produk yang dibeli.
- Rekomendasi Produk yang Relevan: Berdasarkan hasil analisis pola pembelian, solusi yang diusulkan adalah memberikan rekomendasi produk yang relevan kepada pelanggan. Dengan menggunakan teknik seperti collaborative filtering atau content-based filtering, dapat dikembangkan sistem rekomendasi yang dapat memberikan rekomendasi produk yang sesuai dengan preferensi dan pembelian sebelumnya.
- Optimalisasi Strategi Pemasaran: Solusi yang diusulkan adalah menggunakan wawasan yang diperoleh dari analisis pola pembelian untuk mengoptimalkan strategi pemasaran. Hal ini meliputi mengidentifikasi segmen pelanggan yang berbeda berdasarkan pola pembelian mereka, mengembangkan kampanye promosi yang lebih efektif, dan menyesuaikan strategi pemasaran berdasarkan preferensi pelanggan.
- Pengembangan Personalisasi Pengalaman Pelanggan: Solusi yang diusulkan adalah memanfaatkan wawasan tentang pola pembelian untuk meningkatkan personalisasi pengalaman pelanggan. Dengan menggunakan teknik seperti customer segmentation atau customer journey mapping, dapat dikembangkan strategi yang lebih personal dan relevan dalam berinteraksi dengan pelanggan, meningkatkan retensi pelanggan, dan menciptakan pengalaman belanja yang lebih memuaskan.

## Data Understanding

Untuk Proyek ini saya menggunakan data yang berasal dari kaggle.Dataset ini memiliki 8 Atribut,tetapi yang digunakan dalam proyek ini hanya 3.

Dataset yang digunakan: [Online Retail](https://www.kaggle.com/datasets/lakshmi25npathi/online-retail-dataset/data)

### Variabel-variabel pada Online Retail Dataset adalah sebagai berikut:

| Nomer | Variabel    | Tipe Data | Keterangan                         |
| ----- | ----------- | :-------: | ---------------------------------- |
| 1     | Invoice     |  String   | Berisi kode untuk setiap pembelian |
| 2     | StockCode   |  String   | Berisi kode stok                   |
| 3     | Description |  String   | Berisi Item-Item                   |
| 4     | Quantity    |    Int    | Berisi tingkat kualitas            |
| 5     | InvoiceDate |   Date    | Berisi tanggal transaksi           |
| 6     | Price       |    Int    | Berisi harga item                  |
| 7     | Customer ID |  String   | Berisi ID pelanggan                |
| 8     | Country     |  String   | Berisi setiap negara               |
| 9     | month       |   Date    | berisi bulan                       |
| 10    | day         |   Date    | berisi hari teransaksi             |

#### Variabel-variabel pada Online Retail Dataset yang digunakan dalam proyek ini adalah sebagai berikut:

| Nomer | Variabel    | Tipe Data | Keterangan                  |
| ----- | ----------- | :-------: | --------------------------- |
| 1     | Invoice     |  String   | Berisi umur pelanggan       |
| 2     | InvoiceDate |   Date    | Berisi pendapatan pelanggan |
| 3     | month       |   Date    | berisi bulan                |
| 4     | day         |   Date    | berisi hari teransaksi      |

**Rubrik/Kriteria Tambahan (Opsional)**:

- Visualisai Data
  ![Visualisasi menggunakan Seaborn](img/Gambar2.png)
  <br>
  ![Visualisasi menggunakan Seaborn](img/Gambar3.png)
  <br>
  ![Visualisasi menggunakan Seaborn](img/Gambar4.png)
  <br>
  ![Visualisasi menggunakan Seaborn](img/Gambar5.png)
  <br>
  ![Visualisasi menggunakan Seaborn](img/Gambar6.png)
  <br>

## Data Preparation

1. Mencari dataset yang berisi informasi tentang .
2. Mendownload dataset yang sudah dicari dan menload dataset yang akan digunakan.

```python
  !kaggle datasets download -d lakshmi25npathi/online-retail-dataset
```

```python
!unzip online-retail-dataset.zip -d retail
!ls retail
```

```python
  data = pd.read_excel("online_retail_II.xlsx")
```

3. Memilih library yang digunakan.

```python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
from mlxtend.preprocessing import TransactionEncoder
from mlxtend.frequent_patterns import association_rules, apriori
import plotly.express as px
```

4. Fungsi pd.to_datetime() digunakan untuk mengonversi data dari format string ke format datetime

```python
  data['Order Date'] = pd.to_datetime(data['Order Date'], format="%d/%m/%Y %H:%M")
```

5. Membuat kolom baru dari kolom Menggunakan fungsi dt.month, dt.weekday, dan dt.hour untuk mengambil informasi tanggal, bulan, hari dalam satu minggu, dan jam dari kolom 'InvoiceDate'

```python
data["month"] = data['InvoiceDate'].dt.month
data["day"] = data['InvoiceDate'].dt.weekday
data["hour"] = data['InvoiceDate'].dt.hour
data.head()
```

6. Kode untuk mengubah data transaksi menjadi pivot table dan menampilkan ukuran dataset serta beberapa baris pertama dari pivot table tersebut.

```python
item_count_pivot = item_count.pivot_table(index='Invoice', columns='Description', values='Count', aggfunc='sum').fillna(0)
print("Ukuran Dataset:", item_count_pivot.shape)
item_count_pivot.head()
```

7. kode untuk mengambil kolom "Invoice" dan "Description" dari dataframe `data` dan menampilkan 10 baris pertama dari data tersebut.

```python
data = data[["Invoice", "Description"]].copy()
data.head(10)
```

8. Kode untuk mencetak ukuran dataset pivot table, jumlah transaksi, dan jumlah item.

```python
print("Ukuran dataset :", item_count_pivot.shape)
print("Jumlah transaksi :", item_count_pivot.shape[0])
print("Jumlah item :", item_count_pivot.shape[1])
```

## Modeling

Pembuatan model asosiasi untuk menemukan item-item yang sering dibeli bersama

```python
support = 0.02
frequent_items = apriori(item_count_pivot, min_support= support, use_colnames=True)
frequent_items.sort_values("support", ascending=False).head(10)
```

Menentukan nilai support minimum support = 0.02 menetapkan nilai support minimum untuk aturan asosiasi yang akan ditemukan. Support menunjukkan seberapa sering suatu item atau kumpulan item muncul dalam transaksi Nilai 0.02 berarti item atau kumpulan item harus muncul setidaknya dalam 2% dari total transaksi untuk dipertimbangkan dalam pembuatan aturan asosiasi.
Menerapkan Algoritma Apriori Memanggil fungsi apriori() dari library apriori untuk menerapkan algoritma Apriori. Algoritma ini dirancang untuk menemukan aturan asosiasi yang kuat dalam dataset transaksional.
Menampilkan item-item yang sering muncul frq_items.sort_values("support", ascending=False).head(10) menampilkan 10 item atau kumpulan item yang paling sering muncul, diurutkan berdasarkan nilai support dari yang tertinggi ke terendah.

## Visualisasi Model

membuat visualisasi distribusi tiga dimensi dari aturan asosiasi. Kode tersebut menggunakan library seaborn untuk mengatur gaya plot menjadi "whitegrid". Selanjutnya, kode tersebut membuat objek figure dengan ukuran 12x12 dan menambahkan subplot dengan proyeksi 3D ke dalam objek figure. Kemudian, nilai support, confidence, dan lift diambil dari dataframe rules dan disimpan dalam variabel x, y, dan z. Label sumbu x, y, dan z diatur pada plot, dan scatter plot dibuat menggunakan nilai x, y, dan z sebagai koordinat. Judul plot diatur, dan plot ditampilkan. Dengan menggunakan kode tersebut, Anda dapat dengan mudah membuat visualisasi distribusi tiga dimensi dari aturan asosiasi.
![Visualisasi menggunakan Seaborn](img/gambar8.png)

membuat scatter plot dari hubungan antara support, confidence, dan lift dalam aturan asosiasi. Berikut adalah penjelasan singkat dari setiap blok kode tersebut:

1. Blok pertama:

   - Mengimport library seaborn dan matplotlib.pyplot.
   - Membuat figure dengan ukuran 10x6.
   - Menggunakan scatter plot dari seaborn dengan sumbu x = "support", sumbu y = "confidence", dan ukuran titik ditentukan oleh "lift".
   - Menambahkan judul plot, label sumbu x dan y.
   - Menampilkan plot dengan menggunakan plt.show().

2. Blok kedua:

   - Membuat figure dengan ukuran 10x6.
   - Menggunakan scatter plot dari seaborn dengan sumbu x = "support", sumbu y = "lift", dan ukuran titik ditentukan oleh "confidence".
   - Menambahkan judul plot, label sumbu x dan y.
   - Menampilkan plot dengan menggunakan plt.show().

3. Blok ketiga:
   - Membuat figure dengan ukuran 10x6.
   - Menggunakan scatter plot dari seaborn dengan sumbu x = "confidence", sumbu y = "lift", dan ukuran titik ditentukan oleh "support".
   - Menambahkan judul plot, label sumbu x dan y.
   - Menampilkan plot dengan menggunakan plt.show().

Dengan menggunakan kode tersebut, Anda dapat dengan mudah membuat scatter plot yang memvisualisasikan hubungan antara support, confidence, dan lift dalam aturan asosiasi
![Visualisasi ](img/gambar10.png)
![Visualisasi ](img/gambar11.png)
![Visualisasi ](img/gambar12.png)

## Deployment

Link Streamlit : [Online Retail](https://online-retail-appsyhfgwcxjufersppxbip.streamlit.app/)
![Streamlit](img/Gambar1.png)
