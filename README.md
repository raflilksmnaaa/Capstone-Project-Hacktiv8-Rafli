# Analisis Pasar Saham Periode Juni 2025 Berbasis AI Menggunakan IBM GRANITE
Rafli Laksamana <raflilksmnaaa@gmail.com>

## Project Overview

### Latar Belakang
Pasar saham, bisa dibilang sebagai jantung ekonomi modern yang telah lama menjadi tempat arena bagi para investor untuk </dd> mengalokasikan uang modal dan mencari pertumbuhan kekayaan. Biasanya, secara tradisional analisis pasar saham masih mengandalkan data historis,laporan keuangan (lapkeu) dan penilaian fundamental serta teknikal yang dilakukan secara manual atau dengan bantuan software konvensional. Namun, dengan berkembang pesatnya Informasi Teknologi (IT) dan munculnya Big Data, Volume dan kompleksitas informasi yang ada pada pasar saham telah meningkat secara drastis. Dengan segala dinamika dan latar belakang yang telah disebutkan serta capstone projek yang mengharuskan menggunakan IBM Granite, terpikirkan untuk membuat suatu program yang memaanfaatkan kemampuan pemrosesan data dari pustaka seperti **Pandas** dan analisis dari model AI yang canggih seperti **IBM Granite**.

### Tujuan Proyek

#### Menghasilkan statistik ringkasan dan visualisasi ####
diharapkan program ini dapat memberikan gambaran umum data melalui statistik deskriptif dan membuat grafik untuk memahami tren seperti harga saham rata-rata per sektor, distribusi PE Ratio dan hubungan antara kapitalisasi pasar dan volume perdagangan. 
#### Melakukan analisis mendalam menggunakan model AI ibm-granite/granite-3.3-8b-instruct ####
dengan menggunakan model IBM Granite yaitu, ibm-granite/granite-3.3-8b-instruct akan dihasilkan analisis komprehensif terhadap data saham, termasuk tren pasar, analisis sektor, rekomendasi saham (beli/hindari), penilaian resiko dan strategi yang bisa menjadi referensi untuk membuat keputusan. Diakhiri dengan menyimpan output analisis dari model AI ke dalam file teks.

### Permasalahan dan Pendekatan yang dilakukan ###
ada beberapa permasalahan yang saya berusaha pecahkan pada projek dan pendekatan yang saya lakukan. meliputi : Pengolahan Volume Data Pasar Saham Yang Besar dan Kompleks, Mendapatkan Insight dan Findings dari Data Mentah, Mengatasi Keterbatasan Analisis Manual atau Konvensional serta mennyajikan hasil analisis yang terstruktur dan tentu saja mudah dipahami.
#### Pengolahan Volume Data Pasar Saham Yang Besar dan Kompleks ####
seperti yang kita tahu, Data pasar saham sangat dinamis dan bervolume tinggi. Mengolah,membersihkan, dan mempersiapkannya secara manual tentu saja akan sangat memakan waktu dan rentan kesalahan. Makanya, pada projek ini disediakan framework otomatis untuk memuat, memvalidasi, dan memproses data supaya efisien.
#### Mendapatkan Insight dan Findings dari Data Mentah ####
Data mentah yang berupa harga,volume,rasio,dll, secara tidak langsung memberikan kita gambaran tentang tren pasar,kinerja sektor, ataupun potensi resiko. Pada projek ini menggunakan statistik,visualisasi, dan yang paling utama adalah penggunaan model AI ibm-granite/granite-3.3-8b-instruct untuk mendapatkan wawasan lebih dalam dan terstruktur dari data.
#### Mengatasi Keterbatasan Analisis Manual atau Konvensional ####
seperti yang kita tahu, analisis tradisional mungkin terbatas pada pola yang jelas atau indikator standar. Dengan memaanfaatkan model AI ibm-granite/granite-3.3-8b-instruct kita bisa mengidentifikasi pola atau hubungan yang lebih kompleks dalam data yang mungkin terlewat ketika kita menggunakan metode konvensional. Kemudian, dari output analisis data saham yang sangat teknis digunakan Model AI IBM Granite untuk menyajikan hasil analisis dalam format yang lebih mudah dipahami,mencakup ringkasan,rekomendasi, dan strategi yang jelas.

### RAW Dataset ###
Data yang digunakan merupakan data saham dari berbagai sektor pada periode bulan Juni 2025 yang diambil dari Website Kaggle. 

Link : <https://www.kaggle.com/datasets/pratyushpuri/stock-market-june-2025-dataset/data>

### Insight & Finding ###
1. ditemukan dominasi sektor komunikasi dalam Sampel Data Analisis AI, Analisis AI secara spesifik mencatat bahwa dataset sampel (143 baris) yang digunakan untuk analisis ternyata didominasi oleh sektor *Communication Services*, yang menyumbang 91% data sampel tersebut. tentu saja, ini berbeda dengan data asli 1000 baris yang memiliki distribusi sektor lebih merata (walaupun, industrial utilities, dan communication services adalah top 3). menurut saya ini merupakan temuan yang unik karena secara eksplisit diidentifikasi oleh model AI dari data yang dikasih kepads AI tersebut. dari temuan ini, kita mendapatkan insight tentang "risiko" karena berdasarkan temuan mengenai dominasi sektor *Communication Service*, AI secara logis menyimpulkan adanya "Potensi Konsentrasi Risiko". Jika seorang investor hanya berinvestasi pada saham-saham dalam sampel ini (atau jika sampel ini mencerminkan bias dalam data yang lebih besar) maka kinerja portofolio akan sangat bergantung pada keadaan dan tren di satu sektor, jika sektor tersebut mengalami penurunan, maka risiko akan meningkat. dari insight, didapatkan temuan lanjutan sebagai konsekuensi dari insight "resiko" ini. AI merekomendasikan strategi *Diversifikasi* dengan mengalokasikan investasi accross other sectors atau di seluruh sektor lain, dengan tujuan untuk memitigasi risiko.
