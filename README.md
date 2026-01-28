# cek-link-pishing

dataset from Kaggle

- **model_phishing.pkl** : model terlalu "bodoh" FALSE NEGATIF : 4,293 link phishing lolos.

- **xgboost_phising_98acc.pkl** : model terlalu strict, masa "https://www.google.com" dianggap phishing wkwkwk, FALSE NEGATIF : 1,296 link phishing lolos
  yang ini ditambah TF-IDF.




📊 Perbandingan Performa Model

Tabel berikut menunjukkan peningkatan performa antara model lama (XGBoost standar) dan model baru (hasil tuning + fitur NLP):

Metrik	Model Lama (XGB Biasa)	Model Baru (Tuned + NLP)	Improvement
Akurasi	**~95.6%	98%	+2.4%**
Recall (Daya Tangkap Phishing)	**~90%	97%	+7% **(Sangat Signifikan)
False Negative (Link Phishing Lolos)	4.293 link	1.296 link	Turun ~70%

False Negative = phishing yang salah dikira aman

Semakin kecil nilainya, semakin aman sistem

Akurasi naik ke 98%, menunjukkan peningkatan performa keseluruhan tanpa mengorbankan recall.


