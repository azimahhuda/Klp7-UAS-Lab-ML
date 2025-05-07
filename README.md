# Kelompok 7
# Klasifikasi Gambar Intel

## Anggota Tim
- Cut Dahliana (2208107010027) - Membuat style streamlit
- Qandila Ahmara (2208107010039) - Membuat code membangun model
- Della Rahmatika (2208107010041) - Membuat code membangun model, membuat streamlit awal beserta mencari dataset
- Firjatullah Afny Abus (2208107010059) - Membuat slide presentasi
- Azimah Al-Huda (2208107010069) - Merapikan code dan menambahkan markdown

## Deskripsi Proyek

Aplikasi ini merupakan sistem klasifikasi gambar yang menggunakan model Convolutional Neural Network (CNN) untuk mengklasifikasikan gambar dari Intel Image Dataset ke dalam tiga kategori:

- 🏢 *Bangunan* (Buildings)
- 🌿 *Hutan* (Forest)
- 🌊 *Laut* (Sea)

Aplikasi ini dibangun menggunakan framework Streamlit untuk antarmuka pengguna yang interaktif dan intuitif, dengan TensorFlow/Keras sebagai backend untuk model pembelajaran mesin. Pengguna dapat mengunggah gambar pemandangan, dan aplikasi akan menampilkan hasil klasifikasi beserta tingkat kepercayaan model dalam bentuk visualisasi yang informatif.

## Fitur Utama

- Antarmuka pengguna yang responsif dan intuitif
- Klasifikasi real-time dengan visualisasi hasil
- Tampilan distribusi probabilitas untuk setiap kategori
- Desain yang menarik dengan tema biru dan putih
- Indikator kepercayaan berwarna sesuai dengan tingkat akurasi prediksi

## Prasyarat

Sebelum menjalankan aplikasi, pastikan Anda telah menginstal perangkat lunak dan pustaka berikut:

- Python 3.7+
- TensorFlow 2.x
- Streamlit
- Numpy
- Pandas
- Plotly
- PIL (Python Imaging Library)

## Instalasi

1. Clone repositori ini ke komputer lokal Anda:
   bash
   git clone https://github.com/azimahhuda/Klp7-UAS-Lab-ML.git
   cd klasifikasi-gambar-intel
   

2. Buat dan aktifkan lingkungan virtual (opsional tetapi direkomendasikan):
   bash
   python -m venv venv
   
   # Untuk Windows
   venv\Scripts\activate
   
   # Untuk macOS/Linux
   source venv/bin/activate
   

3. Instal semua dependensi yang diperlukan:
   bash
   pip install -r requirements.txt
   

## Persiapan Model

1. Unduh model terlatih dari link berikut: [Model Intel (Google Drive)](https://drive.google.com/drive/folders/1W7Fhp4O7DaMD2Q5c-B9HqPY0pftpczbC?usp=sharing)
2. Simpan file model dengan nama model_intel_best.keras di direktori utama proyek.

## Menjalankan Aplikasi

1. Pastikan semua dependensi telah terinstal dan model telah ditempatkan di lokasi yang benar.
2. Jalankan aplikasi Streamlit:
   bash
   streamlit run depmodel.py
   
3. Aplikasi akan otomatis terbuka di browser web Anda dengan alamat http://localhost:8501.

## Cara Penggunaan

1. Buka aplikasi di browser.
2. Klik pada tombol "Pilih sebuah gambar..." untuk mengunggah gambar pemandangan (format JPG, JPEG, atau PNG).
3. Tekan tombol "Klasifikasikan Gambar" untuk memproses gambar.
4. Lihat hasil klasifikasi dan distribusi probabilitas yang ditampilkan.
5. Tekan tombol "Lihat Detail" untuk melihat informasi probabilitas yang lebih detail.

## Struktur File


klasifikasi-gambar-intel/
├── depmodel.py         # File utama aplikasi Streamlit
├── model_intel_best.keras  # Model terlatih
├── requirements.txt    # Daftar dependensi
└── README.md           # Dokumentasi proyek


## File Requirements.txt

Berikut adalah isi dari file requirements.txt yang diperlukan:


streamlit==1.24.0
tensorflow==2.12.0
numpy==1.23.5
pandas==2.0.2
pillow==9.5.0
plotly==5.15.0


## Pengembangan Lanjutan

Untuk pengembangan lebih lanjut, Anda dapat:

1. Menambahkan lebih banyak kategori gambar ke dalam model
2. Meningkatkan performa model dengan teknik transfer learning
3. Menambahkan fitur untuk menyimpan hasil klasifikasi
4. Implementasi fitur batch processing untuk klasifikasi banyak gambar sekaligus