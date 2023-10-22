# Analisis Sentimen Pengguna Twitter Terhadap Topik Perpajakan Di Indonesia Menggunakan TF-IDF Dan Naive Bayes
Adapun tujuan dari penelitian ini ialah sebagai berikut :
1. Mengukur tingkat sentimen masyarakat pengguna twitter terhadap topik perpajakan pasca serangkaian peristiwa yang secara signifikan menurunkan kepercayaan masyarakat terhadap instansi perpajakan.
2. Mendeskripsikan evaluasi penggunaan metode pembobotan TF-IDF dan Klasifikasi Naive Bayes dalam melakukan analisis sentimen topik perpajakan.

Berdasarkan hasil pelabelan, terdapat 572 tweet dengan sentimen positif, 6706 tweet dengan sentimen negatif, dan 202 tweet dengan sentimen netral. Adapun perbandingan jumlah ketiga kelas sentimen tersebut seperti ditunjukkan oleh grafik berikut

![hasilpelabelan](hasilpelabelan.png)

Proses evaluasi model dilakukan terhadap dua skenario pengujian, yaitu klasifikasi pada data sebelum random under sampling dan setelah mengalami random sampling. Kedua skenario tersebut digunakan untuk menganalisis dan membandingkan performa model dalam mengklasifikasikan data pada kondisi yang berbeda. Hasil perbandingan dari kedua skenario tersebut seperti pada tabel berikut ini.

![hasilpelabelan](matrikskonfusi.PNG)

Hasil penelitian menunjukkan bahwa metode pembobotan TF-IDF dan klasifikasi Naive Bayes dapat digunakan untuk menganalisis sentimen topik perpajakan dengan akurasi sebesar 89.97%, presisi sebesar 46.68%, dan sensitivitas sebesar 33.61%. Namun, hasil analisis pada metrik evaluasi tersebut menunjukkan bahwa model klasifikasi cenderung mengelompokkan data uji ke dalam kelas sentimen negatif, sehingga diperlukan teknik random under sampling untuk menciptakan distribusi yang seimbang antara kelas sentimen positif, netral, dan negatif. Penerapan teknik random under sampling menghasilkan nilai akurasi sebesar 53.28%, presisi sebesar 52.66%, dan sensitivitas sebesar 52.52%. Hasil tersebut menunjukkan bahwa model dapat memberikan hasil prediksi yang lebih seimbang. Namun, model masih menghadapi tantangan dalam mengklasifikasikan data sentimen yang termasuk dalam kelas positif dan netral. Hal tersebut diakibatkan dominasi data tweet dengan kelas negatif

Analisis evaluasi menunjukkan bahwa model dalam penelitian ini masih menghadapi tantangan untuk mengklasifikasikan data sentimen positif dan netral, sehingga perlu mempertimbangkan beberapa saran perbaikan. Adapun saran perbaikan untuk penelitian selanjutnya ialah sebagai berikut :

1. Melakukan penambahan data pada kelas sentimen positif dan netral guna menghindari pembiasan hasil prediksi, mengingat dominasi data sentimen negatif pada penelitian ini.
2. Melakukan pelabelan sentimen dengan mempertimbangkan konteks antar kata dalam sebuah kalimat atau tweet, bukan hanya berdasarkan polaritas kata saja. Hal ini akan meningkatkan akurasi dan ketepatan analisis sentimen.
3. Memperluas analisis dengan mempertimbangkan penggunaan algoritma deep learning seperti Convolutional Neural Networks (CNN), Recurrent Neural Networks (RNN), Long Short-Term Memory (LSTM), Gated Recurrent Unit (GRU), atau metode lainnya untuk menggali konteks antar kata dalam dataset sentimen.

Meskipun demikian, hasil pelabelan sentimen dalam penelitian ini tetap relevan dan dapat digunakan oleh Pemerintah Republik Indonesia, khususnya melalui Direktorat Jenderal Pajak (DJP), untuk memahami pandangan dan sikap masyarakat terhadap layanan perpajakan, sehingga DJP dapat mengambil tindakan yang lebih tepat dan efektif dalam meningkatkan kesadaran serta kepatuhan pajakan di Indonesia.
