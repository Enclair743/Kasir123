# Kasir123 - Aplikasi Point of Sale (POS) 🛒

Aplikasi Kasir berbasis web yang dibangun menggunakan **Streamlit** dengan fitur lengkap untuk mengelola toko/bisnis ritel. Aplikasi ini menyediakan interface yang mudah digunakan untuk kasir dan admin dalam mengelola transaksi, inventori, dan laporan keuangan.

## 🌟 Fitur Utama

### 🔐 Sistem Autentikasi
- **Login Multi-User**: Mendukung role Admin dan Kasir
- **Setup Admin Awal**: Pembuatan akun admin otomatis saat pertama kali digunakan
- **Keamanan Password**: Menggunakan bcrypt untuk enkripsi password
- **Manajemen Profil**: Edit profil pengguna dengan foto profil

### 📊 Dashboard
- **Ringkasan Bisnis**: Jumlah transaksi dan total pendapatan
- **Metrics Real-time**: Data terupdate secara otomatis
- **Interface Modern**: Desain yang bersih dan mudah dipahami

### 📦 Manajemen Barang
- **Tambah Barang**: Input produk dengan kategori, harga, dan stok
- **Edit/Update**: Modifikasi data barang yang sudah ada
- **Hapus Barang**: Penghapusan dengan tracking history
- **Kategori Produk**: Organisasi barang berdasarkan kategori
- **Upload Gambar**: Foto produk untuk identifikasi visual

### 💳 Sistem Transaksi
- **Keranjang Belanja**: Tambah/kurangi item dalam transaksi
- **Metode Pembayaran**: Cash dan QRIS/Transfer
- **Kalkulasi Otomatis**: Total, kembalian, dan pajak
- **Struk Digital**: Generate struk transaksi otomatis
- **Update Stok**: Pengurangan stok otomatis setelah transaksi

### 🕒 Riwayat Transaksi
- **Log Lengkap**: Semua transaksi tersimpan dengan detail
- **Filter dan Pencarian**: Cari berdasarkan tanggal, kasir, atau metode
- **Export Data**: Kemungkinan ekspor untuk backup

### 📈 Laporan dan Statistik
- **Laporan Keuangan**: Pendapatan harian, mingguan, bulanan
- **Grafik Interaktif**: Visualisasi data menggunakan Plotly
- **Analisis Penjualan**: Produk terlaris dan trend penjualan
- **Filter Periode**: Laporan berdasarkan rentang tanggal

### 👥 Manajemen Akun (Admin Only)
- **Tambah Pengguna**: Buat akun kasir baru
- **Role Management**: Pengaturan hak akses pengguna
- **Edit Profil Pengguna**: Kelola data semua pengguna

## 🚀 Instalasi dan Penggunaan

### Persyaratan Sistem
- Python 3.7+
- Streamlit
- Pandas
- bcrypt
- fpdf2
- qrcode
- Pillow
- Plotly

### Langkah Instalasi

1. **Clone Repository**
   ```bash
   git clone https://github.com/Enclair743/Kasir123.git
   cd Kasir123
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   
   Atau install manual:
   ```bash
   pip install streamlit pandas bcrypt fpdf2 qrcode pillow plotly
   ```

3. **Jalankan Aplikasi**
   ```bash
   streamlit run Kasir_app.py
   ```

4. **Akses Aplikasi**
   - Buka browser dan pergi ke `http://localhost:8501`
   - Pada pertama kali, buat akun admin
   - Login menggunakan kredensial admin

## 📱 Screenshot Aplikasi

### Login dan Setup Admin
![Admin Setup](https://github.com/user-attachments/assets/5468d2ee-30c1-4e31-93bc-5ef1efc0d031)

### Dashboard Utama
![Dashboard](https://github.com/user-attachments/assets/36a05349-1c0b-4b58-b57c-d65949a1f454)

### Manajemen Barang
![Manajemen Barang](https://github.com/user-attachments/assets/7fff52a7-5568-4ade-aa49-c9d1a749cb0a)

## 🏗️ Struktur Aplikasi

```
Kasir123/
├── Kasir_app.py          # File utama aplikasi
├── README.md             # Dokumentasi ini
├── requirements.txt      # Dependencies Python
├── .streamlit/           # Konfigurasi Streamlit
├── akun.json            # Database pengguna (auto-generated)
├── barang.json          # Database produk (auto-generated)
├── transaksi.json       # Database transaksi (auto-generated)
└── barang_dihapus.json  # Log barang yang dihapus (auto-generated)
```

## 🔧 Konfigurasi

### File Data JSON
Aplikasi menggunakan file JSON untuk penyimpanan data:
- `akun.json`: Data pengguna dan autentikasi
- `barang.json`: Inventori produk
- `transaksi.json`: Riwayat semua transaksi
- `barang_dihapus.json`: Log barang yang telah dihapus

### Keamanan
- Password di-hash menggunakan bcrypt
- Session management terintegrasi dengan Streamlit
- Validasi input untuk mencegah data corruption

## 👤 Penggunaan

### Untuk Admin:
1. **Setup Awal**: Buat akun admin pertama
2. **Kelola Produk**: Tambah, edit, hapus produk
3. **Buat Akun Kasir**: Tambah pengguna kasir
4. **Monitor Bisnis**: Lihat laporan dan statistik
5. **Kelola Pengguna**: Edit profil semua pengguna

### Untuk Kasir:
1. **Login**: Gunakan kredensial yang diberikan admin
2. **Proses Transaksi**: Tambah item ke keranjang, pilih metode bayar
3. **Cetak Struk**: Generate struk digital untuk pelanggan
4. **Lihat Riwayat**: Akses transaksi yang telah dilakukan
5. **Update Profil**: Edit profil personal

## 🛠️ Teknologi yang Digunakan

- **Frontend**: Streamlit (Python web framework)
- **Data Storage**: JSON files (portable dan mudah dibackup)
- **Authentication**: bcrypt untuk hashing password
- **Charts**: Plotly untuk visualisasi data interaktif
- **PDF Generation**: fpdf2 untuk struk dan laporan
- **QR Code**: qrcode library untuk payment integration
- **Image Processing**: Pillow untuk upload dan resize gambar

## 📄 Lisensi

Proyek ini tersedia untuk penggunaan pembelajaran dan komersial.

## 🤝 Kontribusi

Kontribusi sangat diterima! Silakan buat issue atau pull request untuk perbaikan dan fitur baru.

## 📞 Support

Untuk pertanyaan atau bantuan, silakan buat issue di repository ini.

---

**Kasir123** - Solusi POS sederhana namun powerful untuk bisnis ritel Anda! 🏪✨

---

## English Version

# Kasir123 - Point of Sale (POS) Application 🛒

A web-based POS application built with **Streamlit** featuring comprehensive functionality for managing retail stores/businesses. This application provides an easy-to-use interface for cashiers and administrators to handle transactions, inventory, and financial reports.

## Key Features

- **🔐 Multi-User Authentication**: Supports Admin and Cashier roles
- **📦 Inventory Management**: Add, edit, delete products with categories and stock tracking
- **💳 Transaction Processing**: Shopping cart, multiple payment methods (Cash/QRIS), automatic calculations
- **📊 Dashboard**: Real-time business metrics and summaries
- **📈 Reports & Analytics**: Interactive charts, sales analysis, financial reports
- **👥 User Management**: Admin can create and manage cashier accounts
- **🕒 Transaction History**: Complete transaction logs with filtering capabilities

## Quick Start

1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run the application: `streamlit run Kasir_app.py`
4. Open browser to `http://localhost:8501`
5. Create admin account on first run
6. Start managing your business!

## Technology Stack

- **Frontend**: Streamlit (Python web framework)
- **Data Storage**: JSON files (portable and easy to backup)
- **Security**: bcrypt password hashing
- **Visualization**: Plotly for interactive charts
- **PDF Generation**: fpdf2 for receipts and reports