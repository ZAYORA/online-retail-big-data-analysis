# Online Retail Data Analysis with PySpark

Analisis dataset **Online Retail** menggunakan **Apache PySpark** untuk memahami data transaksi penjualan dan menerapkan beberapa operasi dasar pemrosesan data skala besar.

## 📌 Project Overview

Project ini menggunakan dataset **Online Retail** dari [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/352/online+retail).

Dataset berisi transaksi dari sebuah perusahaan retail online berbasis di Inggris yang menjual berbagai produk hadiah. Data mencakup transaksi pada periode **1 Desember 2010 hingga 9 Desember 2011** dan terdiri dari **541.909 transaksi**.

Pada project ini, dataset diproses menggunakan **PySpark** untuk melakukan eksplorasi dan operasi data seperti filtering, agregasi, sorting, repartitioning, dan pembersihan data.

## 🗂️ Dataset

Dataset yang digunakan:

**Online Retail Dataset — UCI Machine Learning Repository**

* Dataset ID: 352
* Jumlah transaksi: 541.909
* Periode: 2010-12-01 – 2011-12-09
* Format: Excel (`.xlsx`)
* Ukuran file: ±22,6 MB
* Negara utama: United Kingdom

### Dataset Columns

| Column        | Description                   |
| ------------- | ----------------------------- |
| `InvoiceNo`   | Nomor transaksi               |
| `StockCode`   | Kode produk                   |
| `Description` | Nama/deskripsi produk         |
| `Quantity`    | Jumlah produk dalam transaksi |
| `InvoiceDate` | Tanggal dan waktu transaksi   |
| `UnitPrice`   | Harga produk per unit         |
| `CustomerID`  | ID pelanggan                  |
| `Country`     | Negara pelanggan              |

Dataset dapat diunduh melalui:

https://archive.ics.uci.edu/dataset/352/online+retail

> Dataset disediakan oleh UCI Machine Learning Repository dan dilisensikan di bawah **CC BY 4.0**.

## 🛠️ Technologies

Project ini menggunakan:

* Python
* Apache PySpark
* Pandas
* Jupyter Notebook / Google Colab

## 📁 Project Structure

```text
online-retail-pyspark/
│
├── notebook/
│   └── analisis_online_retail.ipynb
│
├── data/
│   └── README.md
│
├── README.md
├── requirements.txt
└── .gitignore
```

## ⚙️ Installation

Clone repository:

```bash
git clone https://github.com/USERNAME/online-retail-pyspark.git
cd online-retail-pyspark
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## 📥 Dataset Setup

Download `Online Retail.xlsx` dari UCI Machine Learning Repository:

https://archive.ics.uci.edu/dataset/352/online+retail

Kemudian letakkan file dataset di folder:

```text
data/Online Retail.xlsx
```

Notebook menggunakan file Excel tersebut sebagai sumber data.

## 🔎 Analysis Performed

Beberapa proses yang dilakukan dalam notebook:

1. Membuat Spark Session.
2. Membaca dataset menggunakan Pandas.
3. Mengubah Pandas DataFrame menjadi PySpark DataFrame.
4. Melihat struktur/schema dataset.
5. Menghitung jumlah data.
6. Menambahkan kolom `TotalPrice`.

```text
TotalPrice = Quantity × UnitPrice
```

7. Melakukan filtering berdasarkan `Quantity`.
8. Memfilter transaksi berdasarkan negara, termasuk France.
9. Melakukan agregasi penjualan berdasarkan `Country`.
10. Menghitung total quantity berdasarkan produk.
11. Mengurutkan transaksi berdasarkan `TotalPrice`.
12. Mengurutkan transaksi berdasarkan `Quantity`.
13. Mengecek jumlah partition Spark.
14. Melakukan repartition menjadi 4 partition.
15. Menampilkan statistik deskriptif.
16. Menghitung jumlah transaksi berdasarkan negara.
17. Menampilkan produk unik.
18. Menghapus data null menggunakan `dropna()`.
19. Menyimpan hasil data yang telah dibersihkan ke CSV.

## 📊 Key Findings

Berdasarkan proses analisis pada notebook:

* **United Kingdom** memiliki jumlah transaksi paling tinggi dibandingkan negara lainnya.
* Terdapat beberapa transaksi dengan nilai `Quantity` yang sangat besar.
* Terdapat transaksi dengan nilai `TotalPrice` yang sangat tinggi.
* Dataset memiliki nilai negatif pada `Quantity` dan `TotalPrice`, yang perlu diperhatikan ketika melakukan analisis lebih lanjut.
* Setelah proses pembersihan menggunakan `dropna()`, data disimpan sebagai output CSV.

## 🚀 Running the Notebook

Notebook dapat dijalankan menggunakan:

* Google Colab
* Jupyter Notebook
* JupyterLab

Jika menggunakan Google Colab, upload dataset `Online Retail.xlsx` terlebih dahulu atau sesuaikan path dataset pada bagian pembacaan data.

Kemudian buka:

```text
notebook/analisis_online_retail.ipynb
```

dan jalankan cell secara berurutan.

## 📚 References

Chen, D. (2015). *Online Retail*. UCI Machine Learning Repository.

Dataset:

https://archive.ics.uci.edu/dataset/352/online+retail

DOI:

https://doi.org/10.24432/C5BW33

## 📄 License

Dataset menggunakan lisensi **Creative Commons Attribution 4.0 International (CC BY 4.0)**.

Copyright and licensing of the dataset belong to the original data provider.
