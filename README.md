# 💳 Credit Risk Analysis Dashboard

Aplikasi web untuk melakukan **prediksi risiko kredit (credit scoring)** menggunakan model **Machine Learning Classification**, dibangun dengan **Streamlit**.

🔗 **Live Demo:** https://credit-scoring-kelompok5.streamlit.app/

---

## 📌 Tentang Project

Project ini bertujuan untuk menganalisis dan memprediksi kemungkinan seorang peminjam mengalami **gagal bayar (Bad Loan)** berdasarkan karakteristik pinjaman, profil peminjam, serta riwayat kredit.

Model dibangun menggunakan data historis pinjaman dan menghasilkan prediksi:

* **Good Loan (0)** → Pinjaman lancar
* **Bad Loan (1)** → Pinjaman berisiko gagal bayar

Aplikasi ini membantu proses evaluasi kredit menjadi lebih cepat dan berbasis data.

---

## 📈 Model Performance

Menggunakan Logistic Regression

| Metric    | Score |
| --------- | ----- |
| Accuracy  | 63%   |
| Precision | 17%   |
| Recall    | 63%   |
| F1 Score  | 27%   |
| ROC-AUC   | 68%   |

---

## 🗂️ Struktur Project

```bash
/
├── model/                  # Folder tempat penyimpanan model
├── .DS_Store
├── Credit_Risk_Management_Analytics.ipynb
├── Dockerfile              # Konfigurasi untuk Docker
├── README.md
├── app.py                  # Main Streamlit application
├── main.py                 # File pendukung aplikasi
├── requirements.txt        # Dependencies
└── schemas.py              # Definisi skema data/input
```
---

## 🔄 Workflow Project

```text
Dataset
   ↓
Data Cleaning
   ↓
Preprocessing
   ↓
Exploratory Data Analysis (EDA)
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Streamlit Deployment
```

---

## 🚀 Cara Menjalankan Lokal

```bash
# 1. Clone repository
git clone https://github.com/difaputri/credit-scoring.git

# 2. Masuk ke folder project
cd credit-scoring

# 3. Buat virtual environment
python -m venv venv

# Windows
venv\Scripts\activate

# Mac/Linux
source venv/bin/activate

# 4. Install dependency
pip install -r requirements.txt

# 5. Jalankan aplikasi
streamlit run app.py
```

Aplikasi akan berjalan di:

```text
http://localhost:8501
```

---

## 🌐 Deployment

Aplikasi telah dideploy menggunakan **Streamlit Community Cloud**.

Setiap perubahan pada branch utama dapat digunakan untuk melakukan update aplikasi.

🔗 Live App:
https://credit-scoring-kelompok5.streamlit.app/

---

## 🛠️ Tech Stack

* **Python**
* **Streamlit**
* **Scikit-Learn**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Plotly**
* **Joblib**

---

## 📊 Dataset

Dataset terdiri dari informasi:

* Loan Characteristics
* Borrower Profile
* Credit History
* Financial Information

### Target Variable

| Variable | Description                 |
| -------- | --------------------------- |
| bad_loan | 0 = Good Loan, 1 = Bad Loan |

---

## ⚠️ Catatan

* Model dibuat untuk tujuan pembelajaran dan analisis akademik.
* Hasil prediksi tidak digunakan sebagai keputusan kredit aktual.
* Beberapa fitur dilakukan preprocessing sebelum masuk ke model.


