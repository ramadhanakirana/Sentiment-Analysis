## Apa itu analisis sentimen 🤔
Analisis sentimen merupakan suatu teknik yang bekerja dengan mengelompokkan polaritas dalam teks yang terdapat dalam kalimat untuk menentukan kelas label sentimen yang cocok dengan data tersebut. Sehingga, dari hasil analisis sentimen akan menggambarkan keadaan emosional seperti kegembiraan, kemarahan, atau kesedihan.

## Metode dan Sumber Data 
Metode yang digunakan dalam analisis ini adalah menggunakan Support Vector Machine dengan data bersumber dari ulasan aplikasi Threads by Instagram pada Google Play Store dari awal diluncurkan hinggal tanggal 20 Juli 2023. Ulasan yang diambil adalah ulasan dengan rating 1 & 2 untuk kelas negatif dan rating 4 & 5 untuk kelas positif. Rating 3 tidak digunakan karena dianggap netral.

## Parameter Evaluasi
Untuk mengevaluasi suatu model, biasanya digunakan beberapa parameter evaluasi. Paraameter evaluasi ini diambil dari confusion matrix. Adapun parameter evaluasi tersebut adalah:
1. Accuracy
   $Accuracy = TP + TN / TP + TN + FP + FN$
3. Recall
4. Precision
5. F1-Score
6. AUC
   
## Tahapan analisis sentimen
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

## Kesimpulan 📃
Berdasarkan analisis yang telah dilakukan (syntax pengerjaan terlampir), maka dapat disimpulkan seperti berikut:


