🎓 Student Performance Tracker

Aplikasi sederhana untuk melacak dan merekap penilaian mahasiswa.
Proyek ini dirancang secara modular sehingga mudah dikembangkan dan dipelihara.

📂 Struktur Direktori
student_performance_tracker/
├── README.md
├── app.py
├── requirements.txt
├── out/
│   ├── report.md
│   └── report.html
└── tracker/
    ├── __init__.py
    ├── __main__.py
    ├── mahasiswa.py
    ├── penilaian.py
    ├── rekap_kelas.py
    └── report.py


Folder seperti .venv/ dan __pycache__/ adalah file lingkungan kerja dan tidak perlu di-push ke repository.

🧠 Deskripsi Modul
File	Deskripsi
app.py	Entry point utama aplikasi. Mengelola alur input → proses → pembuatan laporan
tracker/__main__.py	Entry alternatif (python -m tracker)
tracker/mahasiswa.py	Kelas representasi data mahasiswa (NIM, nama, dll)
tracker/penilaian.py	Logika penilaian (nilai mata kuliah, bobot, validasi)
tracker/rekap_kelas.py	Rekap kelas: rata-rata, jumlah lulus/gagal, statistik
tracker/report.py	Membuat dan menyimpan laporan (Markdown/HTML)
out/report.md	Contoh output laporan yang dihasilkan program
requirements.txt	Daftar dependensi Python proyek
🚀 Cara Menjalankan
1️⃣ Buat & aktifkan Virtual Environment
python -m venv .venv


Windows

.venv\Scripts\activate


Linux / macOS

source .venv/bin/activate

2️⃣ Install dependensi
pip install -r requirements.txt

3️⃣ Jalankan Program
▶️ Via file utama
python app.py

▶️ Via module launcher
python -m tracker

📄 Output Laporan

Laporan otomatis tersimpan di folder out/ dalam format:

.md (Markdown)

.html (bisa dibuka di browser)

🏗️ Status Proyek

✅ Struktur modular
✅ Output laporan
🔜 GUI/web interface (opsional pengembangan ke depan)

✨ Catatan

Pastikan Python 3.10 atau lebih baru

Gunakan gitignore untuk mengabaikan .venv/ & __pycache__/