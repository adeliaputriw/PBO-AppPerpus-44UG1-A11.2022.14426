# 📚 Aplikasi Perpustakaan

Selamat datang di Aplikasi Perpustakaan! 
Aplikasi ini dirancang untuk membantu manajemen perpustakaan, termasuk peminjaman, pengembalian, pencarian buku, dan banyak lagi.

## 🎨 Fitur Utama
- **Transaksi Peminjaman & Pengembalian:**
  - Penambahan buku baru ke dalam database.
  - Pengeditan data buku yang sudah ada.
  - Penghapusan buku yang tidak lagi tersedia.
  - Pencarian buku berdasarkan judul dan penulis.
    
- **Manajemen Anggota:**
  - Penambahan data anggota baru.
  - Pengeditan data anggota yang sudah ada.
  - Penghapusan data anggota.
  - Pencarian anggota berdasarkan nama atau ID anggota.
    
- **Transaksi Peminjaman & Pengembalian:**
  - Pencatatan transaksi peminjaman buku
  - Penghitungan tanggal jatuh tempo pengembalian buku
  - Pencatatan informasi anggota pada saat peminjaman
  - Pencatatan pengembalian buku
  - Pembaruan status buku
  - 
## 🛠️ Instalasi
Langkah-langkah berikut untuk mengatur dan menjalankan aplikasi:

1. **Clone Repository:**
    ```bash
    git clone https://github.com/username/library-app.git
    cd library-app
    ```
2. **Install Dependencies:**
    Pastikan Anda telah menginstal JDK 21 dan JavaFX. Tambahkan JavaFX ke path Anda.
3. **Setup Database:**
   Buat database MySQL dan jalankan skrip berikut untuk membuat tabel `buku`:
    ```sql
    CREATE TABLE transaksi (
      idtransaksi INT(11) PRIMARY KEY,
      idanggota INT(11),
      idbuku INT(11),
      tanggalPinjam DATE,
      tanggalJatuhTempo DATE,
      tanggalKembali DATE,
      status STRING
    );
    ```

    Buat database MySQL dan jalankan skrip berikut untuk membuat tabel `anggota`:
    ```sql
    CREATE TABLE transaksi (
      idtransaksi INT(11) PRIMARY KEY,
      idanggota INT(11),
      idbuku INT(11),
      tanggalPinjam DATE,
      tanggalJatuhTempo DATE,
      tanggalKembali DATE,
      status STRING
    );
    ```

    Buat database MySQL dan jalankan skrip berikut untuk membuat tabel `pustakawan`:
    ```sql
    CREATE TABLE transaksi (
      idtransaksi INT(11) PRIMARY KEY,
      idanggota INT(11),
      idbuku INT(11),
      tanggalPinjam DATE,
      tanggalJatuhTempo DATE,
      tanggalKembali DATE,
      status STRING
    );
    ```
    
    Buat database MySQL dan jalankan skrip berikut untuk membuat tabel `transaksi`:
    ```sql
    CREATE TABLE transaksi (
      idtransaksi INT(11) PRIMARY KEY,
      idanggota INT(11),
      idbuku INT(11),
      tanggalPinjam DATE,
      tanggalJatuhTempo DATE,
      tanggalKembali DATE,
      status STRING
    );
    ```

5. **Konfigurasi Database:**
    Sesuaikan konfigurasi database di `src/main/resources/database.properties`:
    ```properties
    db.url=jdbc:mysql://localhost:3306/nama_database
    db.username=root
    db.password=password_anda
    ```

6. **Jalankan Aplikasi:**
    Buka proyek di IntelliJ IDEA dan jalankan aplikasi.

## 💻 Penggunaan

### Tampilan Transaksi

- **Peminjaman Buku:** Isi detail buku dan anggota, lalu klik `Add`.
- **Pengembalian Buku:** Pilih transaksi dan klik `Edit`, isi tanggal kembali dan update status.
- **Pencarian Transaksi:** Gunakan field pencarian untuk menemukan transaksi berdasarkan ID, buku, atau anggota.

### Tampilan Pencarian Buku

- Gunakan filter pencarian untuk mencari buku berdasarkan judul atau nama penulis.
- Klik pada buku untuk melihat detailnya.


