### Apa itu analisis sentimen 🤔
Analisis sentimen merupakan suatu teknik yang bekerja dengan mengelompokkan polaritas dalam teks yang terdapat dalam kalimat untuk menentukan kelas label sentimen yang cocok dengan data tersebut. Sehingga, dari hasil analisis sentimen akan menggambarkan keadaan emosional seperti kegembiraan, kemarahan, atau kesedihan.

### Metode yang dapat digunakan untuk analisis sentimen 💁‍♀️
Terdapat berbagai macam metode yang dapat dilakukan untuk melakukan analisis sentimen. Antara lain:
1. Support vector machine
2. Naive Bayes classifier
3. K-Nearest Neighbor
dll.

### Cara melakukan analisis sentimen
Cara melakukan analisis sentimen adalah sebagai berikut:
1. Mengumpulkan data/kalimat yang akan dianalisis. Pada project ini digunakan ulasan pengguna aplikasi dari Google Play Store yang diambil melalui teknik scrapping.
2. Melakukan proses preprocessing. Tahapan preprocessing biasanya tergantung dengan data, ada beberapa tahapan yang dibutuhkan ada juga yang tidak dibutuhkan. Urutan pelaksanaannya pun tidak ada aturan khusus. Biasanya preprocessing terdiri dari 5 tahapan yaitu:
   a. Case folding (lowecase kalimat, penghapusan angka dan single character, dll)
   b. Normalization (menormalisasi kata)
   c. Stemming (menghilangkan imbuhan pada kata)
   d. Tokenization (mengubah kalimat menjadi kata yang telah berbentuk 'token')
   e. Stopword removal (menghapus kata yang tidak perlu/tidak penting)
3. Melakukan pembobotan kata. Pembobotan kata dapat menggunakan word2vec maupun TF-IDF. Pada project ini akan digunakan TF-IDF.
4. Menentukan range parameter.
5. Menentukan parameter optimal. Penentuan parameter optimal dapat mencoba satu per satu parameter maupun menggunakan teknik grid search.
6. Melakukan klasifikasi.
7. Penarikan kesimpulan.
