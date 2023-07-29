# Sistem Rekomendasi Film - Aldy Muardi
## Domain Proyek
### Latar Belakang

Dalam era digital yang semakin maju, platform hiburan seperti layanan streaming film dan serial TV telah menjadi sangat populer. Pengguna sekarang memiliki akses ke ribuan film dari berbagai genre, tahun rilis, dan negara. Namun, dengan keberagaman konten yang luas, muncul masalah kelebihan pilihan yang dapat membuat pengguna bingung atau bahkan mengabaikan beberapa film yang mungkin sesuai dengan preferensi mereka. Dalam menghadapi tantangan ini, pengembang platform hiburan telah mengadopsi sistem rekomendasi film yang canggih. 

Sistem rekomendasi film adalah teknologi cerdas yang digunakan oleh platform hiburan untuk memberikan rekomendasi film yang relevan dan menarik kepada pengguna. Tujuannya adalah untuk membantu pengguna menemukan film-film yang sesuai dengan preferensi dan minat mereka, mengatasi masalah kelebihan pilihan, dan meningkatkan pengalaman pengguna secara keseluruhan. Sebuah sistem rekomendasi film biasanya didasarkan pada teknik-teknik pengolahan data dan kecerdasan buatan yang kompleks. Data merupakan komponen kunci dalam sistem ini, dan platform hiburan mengumpulkan beragam informasi, termasuk riwayat penonton, peringkat film, preferensi, ulasan, dan interaksi pengguna sebelumnya dengan konten. Informasi ini dianalisis secara mendalam untuk memahami pola perilaku pengguna dan memprediksi film-film yang mungkin diminati.

Ada beberapa pendekatan yang dapat digunakan dalam mengembangkan sistem rekomendasi film. Salah satunya adalah pendekatan berbasis konten, di mana film-film dianalisis berdasarkan atribut-atribut mereka, seperti genre, aktor, sutradara, plot, dan bahasa. Jika seorang pengguna menyukai film-film dengan genre petualangan dan aktor tertentu, sistem akan merekomendasikan film-film dengan ciri-ciri serupa. Selain itu, ada juga pendekatan berbasis kolaboratif, yang memanfaatkan pola kesamaan antara pengguna. Dalam pendekatan ini, sistem mencari pengguna dengan preferensi serupa dan menggunakan data mereka untuk merekomendasikan film kepada pengguna lain dengan minat yang mirip. Misalnya, jika dua pengguna dengan minat film yang hampir sama memberikan peringkat yang tinggi pada film tertentu, sistem dapat merekomendasikan film tersebut kepada pengguna lain yang memiliki minat yang serupa. Sistem rekomendasi film juga dapat memanfaatkan teknik pembelajaran mesin dan algoritma terbaru. Algoritma ini terus ditingkatkan melalui pembelajaran dari data baru, sehingga sistem dapat menyediakan rekomendasi yang semakin akurat seiring berjalannya waktu.

Kegunaan sistem rekomendasi film tidak hanya menguntungkan bagi pengguna, tetapi juga bagi platform hiburan itu sendiri. Dengan memberikan rekomendasi yang relevan, platform dapat meningkatkan retensi pengguna, meningkatkan waktu tayang, dan mendorong interaksi lebih lanjut dengan konten mereka. Selain itu, data yang dikumpulkan dari interaksi pengguna dengan sistem rekomendasi dapat membantu platform dalam memahami tren dan preferensi pengguna yang sedang berlangsung, sehingga mereka dapat menghadirkan konten baru yang sesuai dengan permintaan pasar.

## _Business Understanding_
Dalam era modern, di mana platform hiburan berbasis streaming telah mengambil alih preferensi penonton, sistem rekomendasi film menjadi kunci untuk mengatasi tantangan kelebihan pilihan dan meningkatkan pengalaman pengguna.

Dengan beragamnya film yang tersedia, pengguna seringkali merasa kewalahan dan bingung dalam memilih konten yang sesuai dengan selera mereka. Sistem rekomendasi film hadir untuk menyelesaikan masalah ini dengan memberikan rekomendasi yang dipersonalisasi berdasarkan pola perilaku dan preferensi pengguna. Pengguna akan merasa diarahkan dengan tepat ke film-film yang paling mungkin mereka nikmati, sehingga meningkatkan kepuasan dan loyalitas pelanggan terhadap platform hiburan tersebut.

Selain meningkatkan pengalaman pengguna, implementasi sistem rekomendasi film memberikan manfaat bisnis yang signifikan. Dengan menarik pengguna untuk terus menggunakan platform, retensi pelanggan meningkat, yang pada gilirannya berdampak positif pada pendapatan dan laba. Informasi yang dikumpulkan dari interaksi pengguna dengan sistem rekomendasi juga memberikan wawasan berharga tentang preferensi dan tren pasar yang dapat digunakan untuk mengoptimalkan strategi konten dan menghadirkan film-film yang diantisipasi oleh pengguna.

### _Problem Statment_
1. Bagaimana meningkatkan akurasi dan efektivitas sistem rekomendasi film untuk memberikan rekomendasi yang lebih personal dan relevan bagi setiap pengguna dengan _content-based filtering_?
2. Bagaimana meningkatkan pengalaman pengguna di platform hiburan dengan menyediakan rekomendasi film yang relevan dan sesuai dengan preferensi masing-masing pengguna dengan _collaborative filtering_?

### _Goals_
1. Menghasilkan rekomendasi film yang dipersonalisasi dan relevan untuk pengguna dengan teknik content-based filtering.
2. Menghasilkan rekomendasi film yang sesuai dengan preferensi pengguna dan belum pernah ditonton sebelumnya dengan collaborative filtering.

### _Solution Statement_
Untuk mencapai goals yang telah ditetapkan, langkah-langkah yang dilakukan oleh penulis adalah sebagai berikut:

1. Data Understanding

Tahap ini melibatkan pemahaman mendalam tentang data yang ada. Data yang relevan untuk sistem rekomendasi film termasuk informasi tentang film-film yang tersedia, preferensi dan riwayat penonton, peringkat film, ulasan, dan interaksi pengguna sebelumnya dengan konten. Penulis menganalisis dan memahami struktur data ini untuk mempersiapkan langkah-langkah selanjutnya.

2. Univariate Exploratory Data Analysis

Tahap ini melibatkan analisis data secara individual untuk memahami distribusi, statistik, dan karakteristik dari setiap atribut data. Dengan melakukan analisis ini, penulis dapat mengidentifikasi potensi outliers, missing values, atau kesalahan data lainnya yang perlu ditangani selama tahap preprocessing.

3. Data Preprocessing

Langkah ini melibatkan pembersihan dan transformasi data agar dapat diolah dengan tepat oleh sistem rekomendasi. Hal ini mencakup penanganan missing values, normalisasi data, penghapusan duplikat, dan penyusunan ulang data agar sesuai dengan kebutuhan model.

4. Data Preparation

Setelah data diproses, tahap ini melibatkan persiapan data yang akan digunakan untuk mengembangkan model rekomendasi. Data yang relevan dipisahkan menjadi data latih dan data uji untuk menguji dan mengevaluasi performa model.

5. Model Development dengan Content-Based Filtering

Dalam langkah ini, penulis mengembangkan model content-based filtering. Model ini menganalisis atribut-atribut film seperti genre, aktor, sutradara, dan plot untuk memberikan rekomendasi film yang mirip dengan film-film yang telah disukai oleh pengguna sebelumnya.

6. Model Development dengan Collaborative Filtering

Selain content-based filtering, penulis juga mengembangkan model collaborative filtering. Model ini menganalisis pola kesamaan antara pengguna untuk merekomendasikan film-film yang disukai oleh pengguna dengan preferensi serupa.

7. Evaluasi dan Peningkatan Model

Setelah mengembangkan kedua model, penulis melakukan evaluasi untuk mengukur kinerja mereka. Model tersebut diperbaiki dan dioptimalkan dengan mengadaptasi feedback dan rekomendasi dari pengguna untuk meningkatkan akurasi dan relevansi rekomendasi.

## _Data Understanding_
Dataset yang digunakan dalam proyek ini merupakan data rekomendasi film. Dataset ini dapat diunduh di [Film Recomendation](https://www.kaggle.com/datasets/uttam94/recommendation). Pada dataset tersebut terdapat 2 file dengan format .csv yang terdiri dari movies.csv dan ratings.csv.

### Variabel-variabel Dataset
1. movies.csv

```
RangeIndex: 9742 entries, 0 to 9741
Data columns (total 3 columns):
 #   Column   Non-Null Count  Dtype 
---  ------   --------------  ----- 
 0   movieId  9742 non-null   int64 
 1   title    9742 non-null   object
 2   genres   9742 non-null   object
dtypes: int64(1), object(2)
```
* moviesId = ID film
* title = Judul film
* genres = genre atau kategori film

2. ratings.csv
```
RangeIndex: 100836 entries, 0 to 100835
Data columns (total 4 columns):
 #   Column     Non-Null Count   Dtype  
---  ------     --------------   -----  
 0   userId     100836 non-null  int64  
 1   movieId    100836 non-null  int64  
 2   rating     100836 non-null  float64
 3   timestamp  100836 non-null  int64  
dtypes: float64(1), int64(3)
```
* userId = ID user
* moviesId = ID film yang telah ditonton
* rating = Rating film
* timestamp = Waktu ketika _user_ melakukan penilaian

### Memahami Isi Dataset
1. Mengetahui jumlah dan tipe dari dataset

Untuk mengentahui informasi dari suatu _data frame_ dapat menggunakan fungsi pandas, yakni `df.info()`

2. Mengetahui nilai unik dataset

Berikut nilai unik yang didapatkan

```
Banyak movie dalam ratings : 9724
Banyak user dalam ratings : 610
```
3. mengetahui jumlah rating

Berikut total rating pada setiap film
**movieId**|**userId**|**rating**|**timestamp**
:-----:|:-----:|:-----:|:-----:	
1|65904|843.0|242914455479
2|36251|377.5|124938583322
3|14747|169.5|52265734386
4|1539|16.5|6290052048
5|14679|150.5|48640552594
...|...|...|...
193581|184|4.0|1537109082
193583|184|3.5|1537109545
193585|184|3.5|1537109805
193587|184|3.5|1537110021
193609|331|4.0|1537157606

## _Data Preparation_
### Menghapus _Missing Value_

_Missing value_ atau nilai yang hilang pada dataset adalah kondisi di mana suatu observasi atau entri dalam dataset tidak memiliki nilai atau informasi yang valid atau lengkap untuk atribut tertentu. Dalam bahasa lain, missing value adalah bagian dari data yang kosong atau tidak diisi.

Berikut jumlah nilai kosong pada setiap variabel:
```
userId       0
movieId      0
rating       0
timestamp    0
title        0
genres       0
dtype: int64
```

### Menghapus Fitur Yang Tidak Diperlukan

Dari fitur yang terdapat pada file ratings.csv, terdapat fitur yang tidak diperlukan, yakni fitur timestap, untuk menghilangkan fitur tersebut dapat menggunakan fungsi `drop()`. Berikut rating setelah fitur timestap dihapus.

Berikut total rating pada setiap film
**#**|**userId**|**movieId**|**rating**
:-----:|:-----:|:-----:|:-----:
0|1|1|4.0
1|1|3|4.0
2|1|6|4.0
3|1|47|5.0
4|1|50|5.0
...|...|...|...
100831|610|166534|4.0
100832|610|168248|5.0
100833|610|168250|5.0
100834|610|168252|5.0
100835|610|170875|3.0
     
### Menghapus Film Yang Tidak Ada Genre
