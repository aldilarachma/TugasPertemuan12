# Sistem Manajemen Buku Perpustakaan

## Tugas Pertemuan 12 - Pemrograman Web II

### Identitas Mahasiswa

* Nama : Aldila Rachma Aulia
* NIM : 60234066
* Mata Kuliah : Pemrograman Web II
* Pertemuan : 12

---

## Deskripsi Project

Project ini merupakan aplikasi Sistem Manajemen Buku Perpustakaan berbasis Laravel yang digunakan untuk mengelola data buku perpustakaan. Aplikasi ini mendukung proses CRUD (Create, Read, Update, Delete), pencarian data, filter kategori, validasi data, bulk delete, serta export data buku ke format CSV.

---

## Fitur Utama

### 1. CRUD Buku

* Menambahkan data buku
* Melihat detail buku
* Mengubah data buku
* Menghapus data buku

### 2. Search dan Filter

* Pencarian berdasarkan judul, pengarang, dan penerbit
* Filter berdasarkan kategori
* Filter berdasarkan tahun terbit
* Filter berdasarkan ketersediaan buku

### 3. Validation Rules Advanced

* Validasi format kode buku menggunakan Custom Validation Rule
* Validasi kategori Programming harus menggunakan bahasa Inggris
* Validasi stok maksimal untuk buku terbit sebelum tahun 2000
* Seluruh pesan validasi menggunakan Bahasa Indonesia

### 4. Bulk Delete

* Memilih beberapa buku sekaligus menggunakan checkbox
* Fitur pilih semua data
* Menghapus banyak data buku dalam satu proses

### 5. Export CSV

* Export seluruh data buku ke file CSV
* File CSV dapat dibuka menggunakan Microsoft Excel atau aplikasi spreadsheet lainnya

### 6. Statistik Buku

* Menampilkan total buku
* Menampilkan jumlah buku tersedia
* Menampilkan jumlah buku habis

---

## Teknologi yang Digunakan

* PHP 8+
* Laravel 12
* MySQL
* Bootstrap 5
* SweetAlert2
* Blade Template Engine

---

## Struktur Database

Tabel utama yang digunakan:

### buku

* id
* kode_buku
* judul
* kategori
* pengarang
* penerbit
* tahun_terbit
* isbn
* harga
* stok
* deskripsi
* bahasa

---

## Screenshot Aplikasi

### 1. Halaman Daftar Buku

<img width="1731" height="3053" alt="01-daftar-buku" src="https://github.com/user-attachments/assets/748dc26b-3d69-4d7b-8e06-bb3cab51b824" />

### 2. Form Tambah Buku

<img width="959" height="479" alt="02-form-tambah-buku" src="https://github.com/user-attachments/assets/99516a45-f0c5-4df0-96be-6d48a3c63366" />

### 3. Validasi Data Buku

<img width="149" height="53" alt="03-validasi-kode-buku 1" src="https://github.com/user-attachments/assets/ce3cf22c-11d0-4f9e-80d4-a639d35ca9ab" />
<img width="412" height="163" alt="03-validasi-kode-buku 2" src="https://github.com/user-attachments/assets/2581bb0b-c1ed-4d8c-8049-2d28cd9f7acf" />

### 4. Detail Buku

<img width="959" height="470" alt="04-detail-buku" src="https://github.com/user-attachments/assets/5796f335-ddad-4ecc-92d5-ec63fb39fd4b" />

### 5. Edit Buku

<img width="959" height="475" alt="05-edit-buku" src="https://github.com/user-attachments/assets/0d6056a4-ee8c-4ec6-88e6-b445ccbb98de" />

### 6. Bulk Delete

<img width="534" height="215" alt="06-bulk-delete" src="https://github.com/user-attachments/assets/4bc725de-c205-4298-bdfe-121faf6298a3" />

### 7. Bulk Delete Berhasil

<img width="610" height="118" alt="07-bulk-delete-berhasil" src="https://github.com/user-attachments/assets/69d1276b-9903-4fd4-b7e9-cd918658cfde" />

### 8. Export CSV

<img width="957" height="175" alt="08-export-csv" src="https://github.com/user-attachments/assets/864a5585-764d-41f3-8ecb-24cf32637a13" />

### 9. Hasil File CSV

<img width="665" height="378" alt="09-isi-csv" src="https://github.com/user-attachments/assets/f464d325-1117-4195-a705-64d9f246f3ac" />

---

## Cara Menjalankan Project

1. Clone repository

```bash
git clone https://github.com/username/repository.git
```

2. Masuk ke folder project

```bash
cd repository
```

3. Install dependency

```bash
composer install
```

4. Copy file environment

```bash
cp .env.example .env
```

5. Generate application key

```bash
php artisan key:generate
```

6. Atur konfigurasi database pada file .env

7. Jalankan migrasi database

```bash
php artisan migrate
```

8. Jalankan aplikasi

```bash
php artisan serve
```

9. Buka browser

```text
http://127.0.0.1:8000
```

---

## Kesimpulan

Pada tugas Pertemuan 12 Pemrograman Web II ini berhasil dibuat aplikasi Sistem Manajemen Buku Perpustakaan berbasis Laravel dengan implementasi Validation Rules Advanced, Bulk Delete Operations, dan Export Data Buku ke CSV. Seluruh fitur berhasil berjalan dengan baik sesuai spesifikasi tugas yang diberikan.
