# Submission 1: Projek-Pengembangan-ML-Pipeline
Nama: Amrul Fadhil Yofan

Username dicoding: amrul_fy

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Detect AI Generated vs Student Generated Text Dataset](https://www.kaggle.com/datasets/prajwaldongre/llm-detect-ai-generated-vs-student-generated-text)) |
| Masalah | Di era kemajuan teknologi seperti sekarang, AI telah mengalami perkembangan yang sangat pesat. Kemajuan ini ditandai dengan adanya suatu sistem AI yang mampu menghasilkan suatu keluaran (output) dalam bentuk tertentu sesuai dengan instruksi dari pengguna. Salah satu bentuk hasil keluaran AI adalah teks. Seiring dengan kemajuan, teks yang dihasilkan oleh AI ini semakin tidak dapat dibedakan secara langsung oleh manusia sehingga muncul suatu isu dalam hal digital texting.   |
| Solusi machine learning | Dengan menggunakan machine learning, model yang dilatih diharapkan dapat menentukan apakah suatu teks  dihasilkan oleh AI atau manusia. |
| Metode pengolahan | Pada dataset yang digunakan, terdapat dua feature, yaitu feature "Text" dan "Label", lalu dilakukan analisis data dengan cara menghapus data kosong dan menerapkan label encoder untuk feature "Label" supaya entri dari data tersebut bertipe integer.  Kemudian dilakukan split data training dan evaluasi menjadi rasio 80:20. |
| Arsitektur model | Arsitektur model yang digunakan yaitu  menggunakan layer TextVectorization sebagai layer yang akan memproses input string kedalam bentuk susunan angka, lalu menerapkan layer Embedding dan LTSM, kemudian memanfaatkan 2 hidden layer dan 1 output layer. |
| Metrik evaluasi | Metrik evaluasi yang digunakan yaitu ExampleCount, AUC, FalsePositives, TruePositives, FalseNegatives, TrueNegatives, dan BinaryAccuracy |
| Performa model | Evaluasi model diperoleh yaitu AUC sebesar 99.958%, kemudian example_count 238, dengan BinaryAccuracy 98.739%, dan loss sebesar 4.454%. Untuk False Negatives 0, False Positive 3, True Negative 111 dan True Positive 124. Model yang telah dibuat memberikan hasil yang baik, tetapi masih dapat dilakukan peningkatan performa karena cenderung overfit dan diperlukan pembaruan data secara berkala.  |
