🚀 Clean Architecture with Python

📋 Tentang Proyek
Proyek ini adalah implementasi Clean Architecture menggunakan Python dan Flask. Dikembangkan sebagai bagian dari kurikulum Software Engineering Academy di Institut Teknologi Bandung (ITB), proyek ini memberikan pengalaman langsung dalam menerapkan arsitektur perangkat lunak yang bersih dan terstruktur.

🏗️ Apa itu Clean Architecture?
Clean Architecture adalah pendekatan desain perangkat lunak yang memisahkan kode menjadi beberapa lapisan, sehingga lebih mudah dipahami, dipelihara, dan diperluas. Prinsip utama Clean Architecture:

Independen dari framework: Tidak terikat dengan teknologi tertentu.
Testable: Mudah diuji secara unit testing.
Independen dari UI & Database: UI atau database bisa diganti tanpa mengubah logika bisnis utama.
🛠️ Teknologi yang Digunakan
Python 3.x
Flask (Micro web framework)
Flask-SQLAlchemy (ORM untuk database)
SQLite / PostgreSQL (Database)
⚙️ Persyaratan Sistem
Python 3.6 atau lebih baru
pip (Python package manager)
Virtual Environment (opsional, direkomendasikan)
🚀 Memulai Proyek
1️⃣ Clone Repository
bash
Copy
Edit
git clone https://github.com/Rivan-Permana/clean-arch-with-python_rivan-permana.git
cd clean-arch-with-python_rivan-permana
2️⃣ Setup Virtual Environment (Opsional, tetapi direkomendasikan)
bash
Copy
Edit
# Membuat virtual environment
python -m venv venv  

# Aktivasi di Windows
venv\Scripts\activate  

# Aktivasi di macOS/Linux
source venv/bin/activate  
3️⃣ Instalasi Dependensi
bash
Copy
Edit
pip install -r requirements.txt
4️⃣ Jalankan Aplikasi
bash
Copy
Edit
python app.py
Aplikasi akan berjalan di http://127.0.0.1:5000/

✅ Pengujian API
Membuat Pengguna Baru
bash
Copy
Edit
curl -X POST http://127.0.0.1:5000/users \
     -H "Content-Type: application/json" \
     -d '{"name": "Jane Doe", "email": "jane@example.com"}'
Mendapatkan Semua Pengguna
bash
Copy
Edit
curl -X GET http://127.0.0.1:5000/users
Mendapatkan Pengguna Berdasarkan ID
bash
Copy
Edit
curl -X GET http://127.0.0.1:5000/users/1
Memperbarui Pengguna
bash
Copy
Edit
curl -X PUT http://127.0.0.1:5000/users/1 \
     -H "Content-Type: application/json" \
     -d '{"name": "Jane Updated", "email": "jane.updated@example.com"}'
Menghapus Pengguna
bash
Copy
Edit
curl -X DELETE http://127.0.0.1:5000/users/1
📁 Struktur Proyek
bash
Copy
Edit
clean-arch-with-python/
├── app.py                 # Entry point aplikasi
├── controllers/           # Direktori controller (handle request)
│   ├── __init__.py
│   └── user_controller.py
├── database/              # Direktori database dan konfigurasi ORM
│   ├── __init__.py
│   └── db_config.py
├── domain/                # Direktori model domain
│   ├── __init__.py
│   └── user.py
├── instance/              # Konfigurasi runtime
├── models/                # Model ORM (SQLAlchemy)
├── repository/            # Layer repository (akses database)
├── routes/                # Definisi endpoint API
├── usecase/               # Logika bisnis aplikasi
├── requirements.txt       # Dependensi proyek
├── .gitignore             # File yang dikecualikan dari Git
└── README.md              # Dokumentasi proyek
🤝 Kontribusi
Kontribusi sangat diterima! Jika Anda ingin berkontribusi:

Fork repository ini
Buat branch baru (feature-xyz)
Lakukan perubahan dan commit
Kirim Pull Request
📜 Lisensi
Proyek ini dilisensikan di bawah MIT License. Lihat file LICENSE untuk detailnya.

📧 Kontak
Jika ada pertanyaan atau masukan, silakan hubungi:
📩 Email: sinarivan99@gmail.com

Dibuat dengan ❤️ oleh Rivan Permana
