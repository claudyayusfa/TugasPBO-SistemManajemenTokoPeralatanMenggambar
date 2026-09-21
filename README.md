# Sistem Manajemen Toko Peralatan Menggambar 🎨 

## Identitas Mahasiswa
- **Nama:** Claudya Yusfa Ariyani
- **NIM:** 2509116043
- **Program Studi:** Sistem Informasi
- **Mata Kuliah:** Pemrograman Berorientasi Objek
- **Dosen Pengampu:** Dr. Akhmad Irsyad S.T., M.Kom.
- **Bahasa Pemrograman:** Java

## 1. Penjelasan Studi Kasus
Program yang dibuat oleh saya adalah Sistem Manajemen Toko Peralatan Menggambar berbasis Command Line Interface atau CLI. Program ini digunakan untuk menampilkan informasi mengenai peralatan menggambar yang tersedia pada sebuah toko. Peralatan menggambar dibagi menjadi dua kategori, yaitu Alat Gambar Konvensional dan Alat Gambar Digital.

Setiap alat gambar memiliki informasi umum berupa kode barang, nama barang, harga barang, dan stok barang.

Selain informasi umum tersebut, setiap kategori memiliki informasi khusus.

### Alat Gambar Konvensional

Memiliki informasi tambahan yaitu jenis barang dan bahan barang. Contoh datanya adalah:

- Pensil 2B
- Pensil Warna Faber Castell (Isi 24 pcs)
- Drawing Pen
- Kuas Lukis
- Cat Air
- Sketchbook

### Alat Gambar Digital

Memiliki informasi tambahan yaitu koneksi barang dan tipe barang. Contoh datanya adalah:

- Drawing Tablet
- Stylus Pen
- Digital Pen
- Pen Display
- XP-Pen Deco

Program menyediakan menu CLI yang dapat memudahkan pengguna untuk melihat sesuai kategori barang, yaitu:

1. Melihat Data Alat Gambar Konvensional
2. Melihat Data Alat Gambar Digital
3. Keluar dari Program

Program dapat menangani input yang tidak sesuai. Jika pengguna memasukkan huruf ketika program meminta pilihan menu, program akan menampilkan pesan bahwa input harus berupa angka dan kembali ke menu utama. 

## 2. Diagram Kelas/Hierarki Class

Hierarki class pada program dapat digambarkan sebagai berikut:

<img width="1844" height="1684" alt="Untitled Diagram drawio (1)" src="https://github.com/user-attachments/assets/a8704ca0-15a0-4d51-a570-bd2bdfa62af1" />

### Penjelasan Class

- AlatGambar
  
  Merupakan superclass yang menyimpan atribut umum yang dimiliki oleh semua alat gambar yaitu kode, nama, harga, dan stok.

  Class ini juga memiliki constructor untuk menginisialisasi data dan method tampilkanInfoAlatGambar() untuk menampilkan informasi umum alat gambar.

- AlatGambarKonvensional

  Merupakan subclass dari AlatGambar. Class ini memiliki atribut tambahan yaitu jenis dan bahan.

- AlatGambarDigital

  Merupakan subclass dari AlatGambar. Class ini memiliki atribut tambahan yaitu koneksi dan tipe.

## 3. Penerapan Inheritance

Inheritance diterapkan dengan membuat class AlatGambar sebagai superclass dan dua class sebagai subclass yaitu AlatGambarKonvensional dan AlatGambarDigital.

### a. Superclass AlatGambar
Class AlatGambar digunakan sebagai superclass karena memiliki informasi yang bersifat umum dan dapat dimiliki oleh semua jenis alat gambar.
  
  <img width="450" height="186" alt="image" src="https://github.com/user-attachments/assets/02314882-285e-4f08-be41-35b495030080" />

### b. Subclass AlatGambarKonvensional
Class AlatGmabarKonvensional merupakan subclass dari AlatGambar.

  <img width="1758" height="324" alt="image" src="https://github.com/user-attachments/assets/d8f38366-e5ca-448a-8250-14f490ea7bbb" />

### c. Subclass AlatGambarDigital
Class AlatGambarDigital juga merupakan subclass dari AlatGambar.

  <img width="1742" height="324" alt="image" src="https://github.com/user-attachments/assets/a335763a-4eca-467d-b414-1c177d7c5518" />

### d. Penggunaan super pada Method
  Selain digunakan untuk memanggil constructor superclass, keyword super juga digunakan untuk memanggil method yang terdapat pada superclass.

  <img width="1010" height="260" alt="image" src="https://github.com/user-attachments/assets/d42cd532-4e21-4add-a82c-cad52852ab19" />

 ### e. Ringkasan Penerapan Inheritance
  - AlatGambar menyimpan data yang umum untuk semua alat gambar.
  - AlatGambarKonvensional mewarisi data umum dari AlatGambar dan menambahkan jenis dan bahan.
  - AlatGambarDigital mewarisi data umum dari AlatGambar dan menambahkan koneksi dan tipe.
  - Keyword extends digunakan untuk membuat hubungan inheritance.
  - Keyword super digunakan untuk memanggil constructor dan method dari superclass.
Dengan penerapan inheritance tersebut, informasi umum tidak perlu dibuat ulang pada setiap class karena dapat diwariskan dari superclass AlatGambar.

## 4. Running Program

Program dijalankan melalui Command Line Interface (CLI). Pada saat program dijalankan, pengguna akan menampilkan menu utama yang terdiri dari tiga pilihan, yaitu melihat alat gambar konvensional, melihat alat gambar digital, dan keluar dari program.

### a. Menu Utama Daftar Peralatan Gambar

Pada menu utama, program menampilkan pilihan menu yang dapat digunakan oleh pengguna. Pengguna dapat memilih menu dengan memasukkan angka 1 sampai 3.

  <img width="538" height="298" alt="image" src="https://github.com/user-attachments/assets/c8ae189e-f111-4105-9304-1dd2cb958847" />

### b. Memilih Menu 1 yaitu Lihat Alat Gambar Konvensional

Jika pengguna memilih menu **1**, program akan menampilkan data alat gambar konvensional yang tersedia.

  <img width="604" height="1020" alt="image" src="https://github.com/user-attachments/assets/a525afd3-33ad-493c-9624-bdf55454ee78" />

### c. Memilih Menu 2 yaitu Lihat Alat Gambar Digital

Jika pengguna memilih menu **2**, program akan menampilkan data alat gambar digital yang tersedia.

  <img width="536" height="1026" alt="image" src="https://github.com/user-attachments/assets/162f3217-a1d5-4fcc-936f-4dabb302e5c2" />

### d. Memilih Menu 3 yaitu Keluar

Jika pengguna memilih menu **3**, program akan menampilkan pesan bahwa program telah selesai dan program akan berhenti.

Pilihan ini digunakan sebagai kondisi untuk menghentikan perulangan menu sehingga pengguna dapat keluar dari program dengan benar.

  <img width="1038" height="582" alt="image" src="https://github.com/user-attachments/assets/5595d881-7c83-42c1-abbf-b896168ee012" />


  


