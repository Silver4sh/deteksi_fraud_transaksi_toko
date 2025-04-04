# Menyimpan isi README dalam bentuk file .md

readme_content = """
# 🕵️‍♂️ Fraud Detection dengan Isolation Forest

Proyek ini bertujuan untuk mendeteksi transaksi mencurigakan (fraud) dalam dataset penjualan menggunakan algoritma **Isolation Forest**. Data dianalisis berdasarkan fitur kuantitas dan nilai transaksi.

## 📂 Isi Proyek
- `fraud_detection.ipynb`: Notebook utama yang berisi proses analisis dan deteksi fraud.
- Dataset: Data transaksi penjualan, termasuk kolom seperti tanggal, nama pembeli, kuantum, nominal, dll.

## 🧠 Metode Deteksi
Model yang digunakan:
- **Isolation Forest**
  - `n_estimators = 100`
  - `contamination = 0.1` *(perkiraan proporsi fraud)*
  - `random_state = 50` *(untuk hasil yang konsisten)*

Fitur yang digunakan untuk pelatihan model:
- `kuantum`
- `fitur2` *(bisa berupa nominal atau variabel lain tergantung dataset)*

## ⚙️ Alur Analisis
1. **Preprocessing**  
   - Membersihkan dan mempersiapkan data untuk analisis.
2. **Model Training**  
   - Melatih Isolation Forest dengan fitur yang dipilih.
3. **Fraud Detection**  
   - Memprediksi transaksi fraud (hasil: -1 untuk fraud, 1 untuk normal).
4. **Ringkasan Fraud**  
   - Menampilkan nama pembeli unik yang terlibat fraud, jumlah transaksi, total kuantum, dan total nominal.

## 📊 Contoh Output Ringkasan Fraud
| nama.pembeli          | jumlah_transaksi | total_kuantum | total_nominal |
|-----------------------|------------------|---------------|----------------|
| TOKO AIDI K.          | 3                | 52940         | 562169860      |
| TOKO ENDANG SUSILAWATI| 2                | 28000         | 297250000      |
| ...                   | ...              | ...           | ...            |

## 🛠️ Teknologi
- Python
- Pandas
- Scikit-learn
- Matplotlib/Seaborn (opsional untuk visualisasi)

## 📌 Catatan
- Pastikan data memiliki kolom yang sesuai: `nama.pembeli`, `kuantum`, `nominal`.
- Parameter model dapat diubah untuk eksperimen lebih lanjut.
"""