🎓 Student Performance Tracker

Aplikasi sederhana untuk melacak dan merekap penilaian mahasiswa. Proyek ini dirancang dengan modular sehingga mudah dikembangkan dan dipelihara.

📂 Struktur Direktori
student_performance_tracker/
├── README.md
├── app.py
├── requirements.txt
├── out/
│ └── report.md
│ └── report.html
└── tracker/
├── **init**.py
├── **main**.py
├── mahasiswa.py
├── penilaian.py
├── rekap_kelas.py
└── report.py

Folder seperti .venv/ dan **pycache**/ adalah artefak environment dan tidak perlu dimasukkan ke repository.

🧠 Deskripsi Modul
File Deskripsi
app.py Entry point aplikasi tingkat atas. Mengatur alur program dari input data hingga pembuatan laporan.
tracker/**main**.py Entry point alternatif (python -m tracker) yang mengikat semua komponen utama.
tracker/mahasiswa.py Kelas representasi mahasiswa (misal: NIM, nama, metode tampilan data).
tracker/penilaian.py Logika penilaian seperti nilai per mata kuliah, validasi, bobot nilai, dll.
tracker/rekap_kelas.py Rekap hasil kelas: rata-rata, jumlah lulus/gagal, statistik nilai.
tracker/report.py Membuat laporan akhir (misal: Markdown) dan menyimpan ke folder out/.
out/report.md Contoh output laporan yang dihasilkan program.
requirements.txt Daftar dependensi Python proyek.
🚀 Cara Menjalankan
1️⃣ Buat dan aktifkan virtual environment
python -m venv .venv

# Linux / macOS

source .venv/bin/activate

# Windows

.venv\Scripts\activate

2️⃣ Instal dependensi
pip install -r student_performance_tracker/requirements.txt

3️⃣ Jalankan aplikasi

# Via file utama

python student_performance_tracker/app.py

# atau via module launcher

python -m student_performance_tracker.tracker
