# AnsariNoor-UTS-PBO2
# Catatan Harian

Catatan Harian adalah aplikasi desktop berbasis Java Swing yang dirancang untuk mencatat kegiatan harian Anda. 
Aplikasi ini memungkinkan pengguna untuk menyimpan, mengedit, mencari, dan menghapus catatan harian dalam file CSV.

## Fitur Utama
1. **Menyimpan Catatan Baru**: Tambahkan catatan dengan judul, isi, dan tanggal.
2. **Edit Catatan**: Pilih catatan yang ada untuk memperbarui detailnya.
3. **Hapus Catatan**: Hapus catatan yang tidak diperlukan.
4. **Pencarian**: Cari catatan berdasarkan judul.
5. **Penyimpanan Data**: Semua data disimpan secara otomatis ke file CSV (`catatan_harian.csv`).

## Struktur File
- `CatatanHarian.java`: File utama yang berisi kode aplikasi.
- `catatan_harian.csv`: File penyimpanan untuk catatan harian.

## Persyaratan
- Java Development Kit (JDK) versi 8 atau lebih baru.
- IDE seperti NetBeans atau IntelliJ IDEA (opsional).
- Library eksternal:
  - **JCalendar**: Library untuk memilih tanggal dalam aplikasi.

## Cara Menjalankan
1. Clone atau unduh proyek ini ke komputer Anda.
2. Pastikan Anda memiliki JDK dan IDE yang sesuai.
3. Buka proyek di IDE Anda.
4. Tambahkan library eksternal JCalendar ke dalam proyek.
5. Jalankan file `CatatanHarian.java`.
6. Aplikasi akan berjalan dengan antarmuka grafis.

## Penjelasan Kode
### Kelas Utama: `CatatanHarian`
Kelas ini merupakan JFrame utama yang menangani semua operasi aplikasi.
- **cekDanBuatFile()**: Mengecek apakah file CSV sudah ada; jika belum, membuat file baru dengan header default.
- **loadCSV()**: Memuat data dari file CSV ke tabel.
- **updateCSV()**: Memperbarui isi file CSV berdasarkan data dari tabel.

### Komponen GUI
- **jTextField1**: Input untuk judul catatan.
- **jTextArea1**: Input untuk isi catatan.
- **jDateChooser1**: Pemilih tanggal.
- **jTable1**: Tabel untuk menampilkan catatan.
- **jButton1 - jButton4**: Tombol untuk simpan, edit, cari, dan hapus.

## Penggunaan
1. Isi judul, isi, dan pilih tanggal pada form input.
2. Klik tombol **Simpan** untuk menambahkan catatan ke tabel.
3. Untuk mengedit, pilih baris pada tabel, ubah data, dan klik tombol **Edit**.
4. Gunakan tombol **Hapus** untuk menghapus catatan yang dipilih.
5. Masukkan judul ke kolom pencarian, lalu klik **Cari** untuk menampilkan hasil yang sesuai.
