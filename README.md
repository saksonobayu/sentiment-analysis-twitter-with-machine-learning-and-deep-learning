# sentiment-analysis-twitter-with-machine-learning-and-deep-learning

change directory of the dataset to run the project



1. Pada project pertama yaitu machine learning

Tahap awal yaitu mengimport library yang dibutuhkan. Selanjutnya membaca dataset yang dimasukkan. Kemudian split dataset menjadi training dan testing dengan test size 10%. Setelah itu memisahkan tweet Positif dan Negatif dari dataset training untuk memvisualisasikan kata-kata yang ada di dalamnya dengan mudah, selanjutnya membersihkan teks dari hashtag, mention dan tautan. kemudian memvisualisasi WordCloud yang hanya menunjukkan kata-kata yang paling tegas dari tweet Positif dan Negatif. Setelah visualisasi, menghapus hashtag, mention, tautan, dan stopwords dari dataset training. Kemudian mengekstrak fitur-fitur yang disebut dengan nltk lib, pertama dengan mengukur distribusi yang sering terjadi dan dengan memilih key yang dihasilkan. Selanjutnya memplot kata-kata yang paling sering didistribusikan. Dengan menggunakan nltk NaiveBayes Classifier, mengklasifikasikan fitur kata tweet yang diekstraksi. Tahap terakhir yaitu menghitung accuracy algoritma. 

2. Pada project kedua yaitu deep learning

Tahap awal yaitu mengimport library yang dibutuhkan. Selanjutnya membaca dataset yang dimasukkan. Selanjutnya menghilangkan sentimen 'Netral' karena tujuannya adalah hanya membedakan tweet positif dan negatif, setelah itu memfilter tweet sehingga hanya teks dan kata yang valid yang tersisa, kemudian mendefinisikan jumlah fitur maksimal sebagai 2000 dan menggunakan Tokenizer untuk memvektorisasi dan mengubah teks menjadi urutan sehingga network dapat menanganinya sebagai input. Selanjutnya menyusun network LSTM, perhatikan bahwa variabel embed_dim, lstm_out, batch_size, droupout_x adalah hiperparameter, perlu perhatikan juga bahwa softmax sebagai fungsi aktivasi, alasannya adalah bahwa network ini menggunakan categorical crossentropy, dan softmax adalah metode aktivasi yang tepat untuk itu. Kemudian split dataset menjadi training dan testing dengan test size 0.33. Selanjutnya training network dengan epoch 7 seharusnya bisa lebih karena laptop yang digunakan kentang. Setelah itu mengekstrakasi validasi data dan menghitung score dan accuracy. Akhirnya mengukur jumlah pengukuran yang benar. Bahwa menemukan tweet negatif berjalan dengan sangat baik untuk network, tetapi memutuskan apakah itu positif atau tidak.

3. Kesimpulan

Dengan machine learning naive bayes algoritma dapat bekerja dengan cukup baik untuk komentar negatif, sedangkan deep learning LSTM bekerja dengan buruk karena dataset training tidak seimbang. Ini dapat diatasi dengan menambah dataset, menggunakan premodel, dan weight class untuk prediksi yang akurat.

source code dan dataset : [https://bit.ly/3EEaZID](https://bit.ly/3ugZtyt)
