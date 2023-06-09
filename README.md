# pertemuan5 

ASSALAMU'ALLAIKUM WR.WB

```s
NAMA    : ALIYAH ASMARANI
NIM     : 312210203
KELAS   : TI.22.A.2
MATKUL  : BASIS DATA
```

# TUGAS PRAKTIKUM 

### 1. Buat sebuah database dengan nama latihan2!

Untuk membuat database gunakan perintah sebagai berikut :

`CREATE DATABASE [nama_database]`

`CREATE DATABASE latihan2;`

lalu, setelah kita membuat database. kita masuk kedalam database tersebut dengan perintah sebagai berikut :

`USE latihan2;`

![gambar1](gambar/1.png)

### 2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam database latihan2!

Untuk membuat Tabel gunakan perintah sebagai berikut :

`CREATE TABLE nama_tabel (nama_field1 tipe _data(ukuran), nama_field2 tipe_data(ukuran), ..., nama_fieldn tipe_data(ukuran));`

`CREATE TABLE biodata (nama VACHAR (15), alamat TEXT);`

![gambar2](gambar/2.png)

### 3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom terakhir!

Untuk menambahkan kolom terakhir yaitu dengan sering digunakan kata AFTER, contoh :

`ALTER TABLE biodata ADD COLUMN keterangan VARCHAR (15) AFTER phone;`

![gambar3](gambar/3.png)

### 4. Tambahkan kolom id(int 11) di awal (sebagai kolom pertama)!

Untuk menambahkan kolom pertama yaitu dengan perintah sebagai berikut :

`ALTER TABLE biodata ADD COLUMN id int(11) FIRST;`

![gambar4](gambar/4.png)

### 5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat!

Untuk menambahkan kolom setelah kolom lain yaitu dengan perintah AFTER 

![gambar5](gambar/5.png)

### 6. Ubah tipe data kolom id menjadi char(11)!

Untuk mengubah type data yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] MODIFY nama_field tipe_data_baru(ukuran);`

![gambar6](gambar/6.png)

### 7. Ubah nama kolom phone menjadi hp (varchar 20)!

Untuk mengubah kolom yaitu dengan perintah sebgai berikut :

`ALTER TABLE [nama_tabel] CHANGE nama_field_lama nama_field_baru tipe_data(ukuran);`

![gambar7](gambar/7.png)

### 8. Tambahkan kolom email setelah kolom hp

![gambar8](gambar/8.png)

### 9. Hapus kolom keterangan dari tabel!

Untuk menghapus kolom dari tabel yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] DROP nama_field;`

![gambar9](gambar/9.png)

### 10. Ganti nama tabel menjadi data_mahasiswa!

Untuk mengganti nama tabel yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] RENAME [nama_tabel_baru];`

![gambar10](gambar/10.png)

### 11. Ganti nama field id menjadi nim!

![gambar11](gambar/11.png)

### 12. Jadikan nim sebagai PRIMARY KEY!

Untuk menambahkan index atau key, gunakan perintah sebagai berikut :
- tipe index :
* PRIMARY KEY
* UNIQUE KEY
* FULLTEXT

`ALTER TABLE [nama_tabel] ADD [INDEX|PRIMARY KEY] (nama_field);`

![gambar12](gambar/12.png)

### 13. Jadikan kolom email sebagai UNIQUE KEY!

Perintah nya sama seperti diatas, hanya saja diganti menjadi UNIQUE KEY

![gambar13](gambar/13.png)


# EVALUASI DAN PERTANYAAN

### Tulis semua perintah-perintah SQL percobaan di pdf praktikum 1 beserta outputnya!

SQL DDL

### * Membuat Database

`CREATE DATABASE latihan1;`

![gambara](gambar/a.png)

### * Membuat Tabel

`CREATE TABLE siswa (nama VARCHAR (100), alamat TEXT);`

![gambarb](gambar/b.png)

### * Menambah Kolom

`ALTER TABLE biodata ADD COLUMN ketengan TEXT AFTER alamat;`

Di perintah yang bapak kasih ada kesalahan yaitu di nama tabelnya. seharusnya siswa bukan biodata.

![gambarc](gambar/c.png)

### * Menambah kolom diawal

`ALTER TABLE siswa ADD COLUMN id INT FIRST;`

![gambard](gambar/d.png)

### * Mengubah nama kolom

`ALTER TABLE siswa CHANGE COLUMN keterangan TO kelas;`

Diperintah ini ada kesalahan, seharusnya yang benar yaitu ini `ALTER TABLE siswa CHANGE keterangan kelas TEXT;` 

![gambare](gambar/e.png)

### * Mengubah tipe data

`ALTER TABLE siswa MODIFY COLUMN kelas VARCHAN(10);`

![gambarf](gambar/f.png)

### * Menghapus kolom

`ALTER TABLE siswa DROP COLUMN kelas;`

![gambarg](gambar/g.png)

### * Menambah PRIMARY KEY

`ALTER TABLE siswa ADD PRIMARY KEY(id);`

![gambarh](gambar/h.png)

### * Menambah CONSTRAINT

`ALTER TABLE siswa ADD CONSTRAINT pk_sisiwa PRIMARY KEY(id);`

Disini sebenarnya tidak bermasalah jika PRIMARY KEY nya kita hapus terlebih dahulu. Jadinya saya coba ganti PRIMARY KEY dengan UNIQUE KEY.

![gambari](gambar/i.png)

### * Menghapus PRIMARY KEY

`ALTER TABLE siswa DROP PRIMARY KEY;`

![gambarj](gambar/j.png)

### * Menghapus CONSTRAINT

`ALTER TABLE siswa DROP CONSTRAINT pk_siswa;`

![gambarj](gambar/j.png)


# APA MAKSUD DARI INT(11)?

INT (11) ADALAH NAMA TIPE DATANYA YAITU INTEGER DAN MEMILIKI PANJANG 11 KARAKTER

# KETIKA KITA MELIHAT STRUKTUR TABEL DENGAN PERINTAH DESC, ADA KOLOM NULL YANG BERISI YES DAN NO. APA MAKSUDNYA?

YAITU UNTUK MENJELASKAN BAHWA PADA RECORD YANG NO HARUS DIISI. SEDANGKAN, YES BISA TIDAK DIISI.







