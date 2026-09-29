# Medical Text Classification: LogisticsRegression, Support Vector Machine (SVM), Random Forest & Adaptive Boosting

Proyek ini bertujuan untuk mengklasifikasikan teks medis (medical/clinical text) menggunakan beberapa algoritma *machine learning* klasik, kemudian membandingkan performanya satu sama lain.

## Deskripsi

Teks medis (misalnya catatan klinis, ringkasan diagnosis, atau dokumen rekam medis) diolah melalui tahapan *text preprocessing* dan *feature extraction*, lalu digunakan untuk melatih beberapa model klasifikasi:

- **Logistic Regression (LR)**
- **Support Vector Machine (SVM)**
- **Random Forest (RF)**
- **Boosting** (mis. AdaBoost / Gradient Boosting / XGBoost)

Tujuannya adalah untuk melihat model mana yang paling efektif dalam mengklasifikasikan kategori teks medis berdasarkan metrik evaluasi seperti akurasi, precision, recall, dan F1-score.

## Struktur Repository

```
Medical_Text_Classification_LR_SVM_RF_Boosting/
├── models/                     # Model hasil training yang telah disimpan
└── medical_text_project.ipynb  # Notebook utama: preprocessing, training, evaluasi
```

## Alur Kerja (Workflow)

1. **Data Loading** — memuat dataset teks medis.
2. **Text Preprocessing** — pembersihan teks (case folding, stopword removal, tokenisasi, stemming/lemmatization).
3. **Feature Extraction** — mengubah teks menjadi representasi numerik (mis. TF-IDF / Bag-of-Words).
4. **Model Training** — melatih model LR, SVM, RF, dan Boosting pada data yang sudah diproses.
5. **Evaluation** — membandingkan performa keempat model menggunakan metrik klasifikasi standar (accuracy, precision, recall, F1-score, confusion matrix).
6. **Model Saving** — menyimpan model terbaik ke folder `models/`.

## Library yang Digunakan

- Python
- Jupyter Notebook
- scikit-learn (Logistic Regression, SVM, Random Forest, Boosting)
- pandas & numpy
- NLTK / library NLP lainnya untuk preprocessing teks

## Cara Menjalankan

1. Clone repository ini:
   ```bash
   git clone https://github.com/febryofibonacciamadeo/Medical_Text_Classification_LR_SVM_RF_Boosting.git
   cd Medical_Text_Classification_LR_SVM_RF_Boosting
   ```
2. Install dependensi yang dibutuhkan (disarankan menggunakan virtual environment):
   ```bash
   pip install numpy pandas scikit-learn nltk jupyter
   ```
3. Buka dan jalankan notebook:
   ```bash
   jupyter notebook medical_text_project.ipynb
   ```

## Hasil

Bandingkan performa keempat model berdasarkan hasil evaluasi di dalam notebook untuk menentukan algoritma yang paling optimal untuk kasus klasifikasi teks medis ini.

## Catatan

README ini disusun berdasarkan struktur file di repository. Silakan sesuaikan bagian dataset, hasil evaluasi (skor akurasi/F1), dan detail preprocessing sesuai isi notebook Anda agar lebih akurat.

## Lisensi

Belum ada lisensi ditentukan. Tambahkan file `LICENSE` jika ingin membuat proyek ini open-source secara resmi.
