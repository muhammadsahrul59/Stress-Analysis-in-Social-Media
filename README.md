# Stress Analysis in Social Media

![Stress_Sosmed](https://github.com/muhammadsahrul59/Stress-Analysis-in-Social-Media/assets/101655285/57410820-1659-4c0a-8e40-713c0d4f0c71)

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Stress Analysis in Social Media](https://www.kaggle.com/datasets/ruchi798/stress-analysis-in-social-media) |
| Masalah | stres merupakan suatu hasil proses transaksi antara manusia (faktor internal) dan lingkungan (faktor eksternal) yang bersifat saling mempengaruhi dan dipengaruhi, dan didalamnya terdapat kesenjangan antara tuntutan dari luar dan sumber daya yang dimiliki oleh manusia. Beberapa ahli menilai hubungan secara daring ini kurang memuaskan dari sisi emosional, sehingga dapat meningkatkan stress ketika merasa terisolasi secara sosial. Semakin sedikit seseorang terhubung dengan manusia lain secara mendalam dan empatik, maka semakin sedikit pula kamu mendapatkan manfaat dari interaksi sosial.|
| Solusi machine learning | Stress susah dilihat dari keseharian seseorang, oleh karena itu dengan machine learning dapat mengetahui apakah seseorang stress hanya dari ketikan seseorang yang dilakukan dimedia sosial |
| Metode pengolahan | Pada data Human Stress Prediction, terdapat tujuh feature, tetapi yang digunakan pada proyek ini hanya feature text dan label, sehingga features selain itu akan dihapus, kemudian dilakukan split data training dan eval menjadi rasio 80:20, dan mengubah data feature menjadi lowercase serta feature label menjadi integer |
| Arsitektur model | Arsitektur model yang digunakan yaitu model embedding dimana terdiri dari vectorize_layer, kemudian layer embedding dengan dimensi embedding yaitu 16, setelah itu layer AveragePooling1D karena data merupakan bentuk text, kemudian layer dense 64, 32 dengan activation relu dan sigmoid karena akan dilakukan klasifikasi antar dua label. Loss yang digunakan binary_crossentropy dengan optimizer Adam dan metrik BinaryAccuray |
| Metrik evaluasi | Metrik evaluasi yang digunakan yaitu ExampleCount, AUC, FalsePositives, TruePositives, FalseNegatives, TrueNegatives, dan BinaryAccuracy |
| Performa model | Evaluasi model diperoleh yaitu AUC sebesar 82%, kemudian example_count 575, dengan BinaryAccuracy 75%, dan loss sebesar 1.364. Untuk False Negatives 68, False Positive 75, True Negative 201 dan True Positive 231. Model yang telah dibuat dapat dilakukan peningkatan performa, karena model belum cukup baik karena BinaryAccuracy masih dibawah 80% |
