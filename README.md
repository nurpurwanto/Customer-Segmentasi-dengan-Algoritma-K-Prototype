# Customer Segmentasi dengan Algoritma K Prototype

Perusahaan sedang berusaha untuk mengenal lebih baik pelanggannya. Tujuannya agar perusahaan dapat membuat strategi pemasaran yang lebih tepat dan juga efisien bagi tiap-tiap pelanggan. 

Salah satu teknik yang bisa dilakukan untuk mengenal lebih baik pelanggan adalah dengan melakukan segmentasi pelanggan. Yaitu dengan mengelompokkan pelanggan-pelanggan yang ada berdasarkan kesamaan karakter dari pelanggan tersebut. Untuk melakukan hal tersebut Kita akan menggunakan teknik unsupervised machine learning.

Salah satunya teknik yang dapat digunakan adalah pengaplikasian machine learning menggunakan algoritma K-Prototypes.  Algoritma K-Prototypes merupakan gabungan dari K-Means dan juga K-Modes yang dapat digunakan untuk melakukan segmentasi dengan data.


Dataset yang kita gunakan memiliki tujuh kolom dengan penjelasan sebagai berikut:
Customer ID			      : Kode pelanggan dengan format campuran teks CUST- diikuti angka.
Nama Pelanggan		    : Nama dari pelanggan dengan format teks tentunya.
Jenis Kelamin		      : Jenis kelamin dari pelanggan, hanya terdapat dua isi data kategori yaitu Pria dan Wanita.
Umur				          : Umur dari pelanggan dalam format angka.
Profesi			          : Profesi dari pelanggan, juga bertipe teks kategori yang terdiri dari Wiraswasta, Pelajar, Professional, Ibu Rumah Tangga, dan Mahasiswa.
Tipe Residen			    : Tipe tempat tinggal dari pelanggan kita, untuk dataset ini hanya ada dua kategori: Cluster dan Sector.
Nilai Belanja Setahun	: Merupakan total belanja yang sudah dikeluarkan oleh pelanggan tersebut.


Exploratory Data Analysis
- Rata-rata dari umur pelanggan adalah 37.5 tahun
- Rata-rata dari nilai belanja setahun pelanggan adalah 7,069,874.82
- Jenis kelamin pelanggan di dominasi oleh wanita sebanyak 41 orang (82%) dan laki-laki sebanyak 9 orang (18%)
- Profesi terbanyak adalah Wiraswasta (40%) diikuti dengan Professional (36%) dan lainnya sebanyak (24%)
- Dari seluruh pelanggan 64% dari mereka tinggal di Cluster dan 36% nya tinggal di Sektor


Feature Engineering:
- Standarisasi Kolom Numerik (Kolom Umur, NilaiBelanjaSetahun)
- Konversi Kategorikal Data dengan Label Encoder (Jenis Kelamin, Profesi, Tipe Residen)


5 Cluster (Segmentasi) hasil clustering K-Prototype

Cluster 0: Diamond Young Entrepreneur, wiraswasta rata-rata nilai transaksi mendekati 10 juta, umur 18 - 41 tahun 
Cluster 1: Diamond Senior Entrepreneur, wiraswasta rata-rata nilai transaksi  mendekati 10 juta. umur  45 - 64 tahun 
Cluster 2: Silver Students, pelajar dan mahasiswa rata-rata umur 16 tahun dan nilai belanja setahun 3 mendekati juta.
Cluster 3: Gold Young Member, profesional dan ibu rumah tangga yang berusia muda umur sekitar 20 - 40 tahun dan nilai belanja setahunnya mendekati 6 juta.
Cluster 4: Gold Senior Member, profesional dan ibu rumah tangga yang berusia umur 46 - 63 tahun dan nilai belanja setahunnya mendekati 6 juta.
