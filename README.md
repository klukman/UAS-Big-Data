# UAS-Big-Data
Lukman Arisandi 21.21.1521

Link data set : https://archive-beta.ics.uci.edu/ml/datasets/online+retail

LATAR BELAKANG
Laporan ini dibuat dengan berdasar pada studi kasus online retail 
dimana data yang dipakai bertipe time series yang kemudian akan dilakukan 
proses EDA serta menacri korelasi antar dataset untuk mengetahui regresi 
antar variable dalam sebuah data. Untuk data yang digunakan terdiri dari 
541909 index serta 8 kolom atribut (InvoiceNo, StockCode, Description, 
Quantity, InvoiceDate, UnitPrice, CustomerID , Country)
kumpulan data transnasional yang berisi semua transaksi yang 
terjadi antara 01/12/2010 dan 09/12/2011 untuk ritel online non-toko yang 
berbasis di Inggris dan terdaftar.
2. ATTRIBUTE INFORMATION:
1. Invoiceno: invoice number. Nominal, a 6-digit integral number uniquely 
assigned to each transaction. If this code starts with letter 'c', it indicates 
a cancellation.
2. Stockcode: product (item) code. Nominal, a 5-digit integral number 
uniquely assigned to each distinct product.
3. Description: product (item) name. Nominal.
4. Quantity: the quantities of each product (item) per transaction. Numeric.
5. Invoicedate: invice date and time. Numeric, the day and time when each 
transaction was generated.
6. Unitprice: unit price. Numeric, product price per unit in sterling.
7. Customerid: customer number. Nominal, a 5-digit integral number 
uniquely assigned to each customer.
8. Country: country name. Nominal, the name of the country where each 
customer resides

Langkah-langkah yang dilakukan pada pengerjaan tugas akhir ini yaitu :
a. Import library yang akan di gunakan dan import dataset
b. Melakukan proses Exploratory Data Analyis, diantaranya
a. Cek info dataset
b. Missing value handling
c. Menangani data outlier
c. Mengecek korelasi antar kolom dengan metode pearson dan spearman
d. Kolom tanggal dijadikan sebagi index
e. dan, pembetukan model regresi menggunakan metode ARIMA
ARIMA adalah singkatan dari Autoregressive Integrated Moving 
Average. Ini adalah algoritma yang digunakan untuk peramalan Time 
Series Data. Model ARIMA memiliki tiga parameter seperti ARIMA(p, d, 
q). Di sini p, d, dan q didefinisikan sebagai:
1. p adalah jumlah nilai tertinggal yang perlu ditambahkan atau 
dikurangi dari nilai (kolom label). Ini menangkap bagian 
autoregresif dari ARIMA.
2. d mewakili berapa kali data perlu dibedakan untuk menghasilkan 
sinyal stasioner. Jika data stasioner, nilai d harus 0, dan jika data 
musiman, nilai d harus 1. d menangkap bagian integral dari ARIMA.
3. q adalah jumlah nilai tertinggal untuk istilah kesalahan yang 
ditambahkan atau dikurangi dari nilai (kolom label). Ini menangkap 
bagian rata-rata bergerak dari ARIMA
