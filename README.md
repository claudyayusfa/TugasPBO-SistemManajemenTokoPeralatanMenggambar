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
- Pensil Warna Fabel Castell (Isi 24 pcs)
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

<img width="1404" height="1044" alt="Untitled Diagram drawio" src="https://github.com/user-attachments/assets/bac3776f-e61f-4b34-88b5-c1ac0a09d41d" />

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

- Superclass AlatGambar memiliki atribut umum:
  
  <img width="450" height="186" alt="image" src="https://github.com/user-attachments/assets/02314882-285e-4f08-be41-35b495030080" />

- Subclass AlatGambarKonvensional

  <img width="1758" height="324" alt="image" src="https://github.com/user-attachments/assets/d8f38366-e5ca-448a-8250-14f490ea7bbb" />

- Subclass AlatGambarDigital

  <img width="1742" height="324" alt="image" src="https://github.com/user-attachments/assets/a335763a-4eca-467d-b414-1c177d7c5518" />

- Penggunaan Method Superclass
  Keyword super digunakan untuk memanggil method dari superclass.

  <img width="1010" height="260" alt="image" src="https://github.com/user-attachments/assets/d42cd532-4e21-4add-a82c-cad52852ab19" />

## 4. Running Program

- Menu Utama Daftar Peralatan Gambar

  <img width="538" height="298" alt="image" src="https://github.com/user-attachments/assets/c8ae189e-f111-4105-9304-1dd2cb958847" />

- Memilih Menu 1 yaitu Lihat Alat Gambar Konvensional

  <img width="604" height="1020" alt="image" src="https://github.com/user-attachments/assets/a525afd3-33ad-493c-9624-bdf55454ee78" />

- Memilih Menu 2 yaitu Lihat Alat Gambar Digital

  <img width="536" height="1026" alt="image" src="https://github.com/user-attachments/assets/162f3217-a1d5-4fcc-936f-4dabb302e5c2" />

- Memilih Menu 3 yaitu Keluar

  


