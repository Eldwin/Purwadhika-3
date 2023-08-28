# Purwadhika-3
Project Capstone 3 - Travel Insurance
## Data Travel Insurance : [https://drive.google.com/drive/folders/1WodnBbuYTvsF0-6HTuQABQ0KCS31lqbK](https://drive.google.com/drive/folders/1iVx5k6tWglqfHb05o0DElg8JHg7VVG_J?usp=drive_link)https://drive.google.com/drive/folders/1iVx5k6tWglqfHb05o0DElg8JHg7VVG_J?usp=drive_link

# Problem Statement :
Perusahaan ingin mengetahui customer mana saja yang akan mengajukan klaim asuransi untuk pertanggungan

# Data Cleansing
Secara umum, kita bisa melihat bahwa:
*Dataset Travel Insurance memiliki 11 kolom dan 4.4328 Baris.
*Hapus Kolom Gender yang tidak terpakai.
*Pembuatan Kelompok Group Age
*Pembuatan Kelompok Duration
*Pembersihan kolom Net Sales

# Data Preparation
1. Merubah fitur/kolom `Agency` menggunakan Binary Encoding.
2. Merubah fitur/kolom `Agency Type` menggunakan One Hot Encoding.
3. Merubah fitur/kolom `Distribution Channel` menggunakan One Hot Encoding.
4. Merubah fitur/kolom `Product Name` menggunakan Binary Encoding.
5. Merubah fitur/kolom `Destination` menggunakan Binary Encoding.
6. Merubah fitur/kolom `Group_Age` menjadi integer 0-4 dengan Ordinal Encoding.
7. Merubah fitur/kolom `Group_Duration` menjadi integer 0-4 dengan Ordinal Encoding.

# Conclusion & Recommendation
## Conclusion
Model kita dapat membaca 82% customer yang tidak melakukan claim asuransi, dan model kita dapat mendapatkan 69% customer yang melakukan claim asuransi.
Dikarenakan pencairan asuransi berbeda-beda, tergantung produk yang diambil.
Untuk proses perhitungan kita asumsikan, 1x pencairan asuransi biaya yang dikeluarkan oleh perusahaan adalah 100 USD.
Anggap saja kita punya 100 customer maka :
*Tanpa Model (semua customer kita asumsikan akan melakukan claim asuransi)
- Total Dana yang perlu disiapkan => 100 x 100 USD = 10.000 USD
*Dengan Model (hanya customer yang diperkirakan melakukan claim asuransi)
- Total Dana yang perlu disiapkan => 69 x 100 = 6.900 USD

Berdasarkan contoh hitungan tersebut, terlihat bahwa dengan menggunakan model kita, maka perusahaan tersebut dapat menyimpan dana sebesar 31% untuk keperluan yang lain.

## Recommendation
- Menambah banyaknya data customer yang melakukan claim asuransi
- Menambahkan fitur2 atau kolom2 baru yang kemungkinan bisa berhubungan dengan claim asuransi, seperti  
  tanggal claim asuransi (untuk melihat ada atau tidak di bulan2 tertentu berkorelasi dengan banyaknya claim 
  asuransi yang masuk) dan ID Customer (untuk melihat customer yang melakukan claim asuransi apakah 
  new_customer atau customer lama yang sudah berlangganan travel asuransi)
- Menganalisa data-data yang model kita masih salah tebak untuk mengetahui alasannya dan karakteristiknya 
  bagaimana.



