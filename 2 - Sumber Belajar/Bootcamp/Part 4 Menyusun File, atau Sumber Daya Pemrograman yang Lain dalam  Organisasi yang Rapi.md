
Tanggal Pembuatan : 23-06-202520:30

Status : ~~finished~~

Tag : [[VSGA]], [[Web Development]]

#### Mengidentifikasi prinsip-prinsip organisasi kode program yang baik.
##### Clean code : 
 sebuah gaya penulisan kode yang memprioritaskan kejelasan, keterbacaan, dan pemeliharaan. Clean code dapat dengan mudah dimengerti oleh pengembang lain yang bekerja dalam proyek yang sama, dan lebih mudah untuk diuji, diperbaiki, dan diperbarui.

##### Prinsip utama dari clean code, antara lain:
**− Keterbacaan (Readability):** Kode harus mudah dibaca oleh manusia. Penggunaan nama variabel, fungsi, dan kelas yang deskriptif dan pemformatan kode yang konsisten adalah kunci untuk meningkatkan keterbacaan.  
**− Sederhana (Simplicity):** Kode harus sederhana, tidak lebih kompleks dari yang diperlukan. Hindari penambahan fitur yang tidak perlu atau teknik yang berlebihan. Prinsip "Keep It Simple, Stupid" (KISS) berlaku di sini.  
**− Konsistensi (Consistency):** Menjaga gaya dan konvensi kode program (koding) yang konsisten di seluruh proyek. Ini melibatkan penggunaan indentasi yang seragam, gaya penulisan variabel yang konsisten, dan sebagainya.  
**− Efisiensi (Efficiency):** Kode harus efisien dari segi waktu dan sumber daya. Menghindari penggunaan operasi atau algoritma yang tidak efisien.  
**− Mudah diuji (Testability):** Clean code harus mudah diuji. Ini berarti bahwa fungsi atau modul harus terisolasi dengan baik dan dapat diuji secara independen, memudahkan pengujian otomatis.  
**− Komposisi (Composition):** Kode harus dapat disusun (composed) dengan baik, memungkinkan pengembang untuk menggabungkan bagian-bagian kecil untuk menciptakan solusi yang lebih besar.  
**− Pembagian Tanggung Jawab (Separation of Concerns):** Prinsip ini berfokus pada membagi program menjadi bagian-bagian yang lebih kecil dengan tanggung jawab tertentu, sehingga setiap bagian hanya bertanggung jawab untuk satu aspek tertentu.  
**− Meminimalkan Duplikasi (DRY - Don't Repeat Yourself):** Hindari duplikasi kode sebisa mungkin. Duplikasi tidak hanya sulit dipelihara, tetapi juga meningkatkan peluang kesalahan.  
**− Menggunakan Komentar yang Efektif:** Komentar seharusnya memberikan nilai tambah dan menjelaskan mengapa suatu keputusan diambil, bukan sekadar mengulangi apa yang sudah jelas dalam kode.  
**− Ketepatan Nama (Meaningful Names):** Memberikan nama variabel, fungsi, dan kelas yang mencerminkan tujuan atau fungsi sebenarnya.

##### Manfaat Clean Code
**− Mudah Dipaham**
**− Meminimalkan Kesalahan (Bugs)**
**− Mempercepat Pengembangan**
**− Memudahkan Pemeliharaan:**
**− Mudah Diuji**
**− Meningkatkan Kolaborasi Tim**
**− Meminimalkan Duplikasi Kode**
**− Keterbacaan (readability) Tinggi**
**− Peningkatan Keterandalan**
**− Peningkatan Kepuasan Pengguna**
**− Efisiensi dalam Debugging**

#### Mengenali dan menerapkan praktik-praktik terbaik dalam menyusun fungsi.
##### 1. Pemberian Nama yang Baik
**− Deskriptif:** Nama harus mencerminkan tugas atau tujuan utama fungsi atau prosedur.  
**− Singkat dan Jelas:** Pilih nama yang singkat namun jelas menggambarkan aksi atau hasil yang diharapkan.  
**− Gunakan Kata Kerja:** Gunakan kata kerja yang memberikan indikasi bahwa fungsi melakukan suatu tindakan.  
**− Hindari Singkatan yang Membingungkan:** Jika perlu, gunakan singkatan yang umum dan dapat dimengerti oleh programmer lain.  
**− Ikuti Konvensi Penamaan:** Gunakan konvensi penamaan yang konsisten, seperti camelCase atau snake_case, sesuai dengan standar komunitas PHP.  
**− Konsisten dalam Gaya Penamaan:** Gunakan gaya penamaan yang konsisten di seluruh program.  

##### 2. Tips dalam Pemberian Nama
**-  Jangan Takut Menulis Nama yang Panjang:**Lebih baik memiliki nama yang panjang dan jelas daripada nama yang ambigu.
**- Gunakan Bahasa atau istilah yang Baku:** Jika memungkinkan, utamakan menggunakan bahasa Inggris, agar bisa dipahami oleh banyak pihak. Hindari penggunaan bahasa lokal atau singkatan yang tidak universal.  
**- Hindari Nama Variabel yang Terlalu Umum:** Nama variabel yang terlalu umum seperti $data atau $temp dapat membingungkan.  
**- Pilih Nama yang Menyiratkan Tipe Data atau Isi Variabel:** Misalnya, $angka, $string, atau $arrayData.  
**- Perbarui Nama Saat Kode Berkembang:** Jika fungsionalitas berubah, pastikan nama tetap mencerminkan tujuan saat ini. Jika tujuan atau fungsi variabel berubah, pastikan untuk memperbarui nama variabel.
#### Membuat struktur file dan direktori yang terorganisir dengan baik.
#### Komentar 
**Komentar Satu Baris:** Gunakan tanda “//” untuk komentar satu baris.
**Komentar Multibaris:** Gunakan tanda “/* */” untuk komentar yang melibatkan beberapa baris

Tujuan Komentar :
Deskripsi : Memberikan penjelasan tujuan umum dari suatu bagian, fungsi, atau prosedur
Keterangan Logika Internal : Memberikan penjelasan langkah-langkah atau keputusan logika yang diambil dalam fungsi atau prosedur

#### Organisasi Folder
Pastikan dalam mengorganisasi folder menggunakan prinsip yang baik seperti repository pattern jika project laravel

#### Readme
Jenis penggunaan file readme:  
− Petunjuk konfigurasi.  
− Petunjuk instalasi.  
− Petunjuk pengoperasian.  
− Sebuah berkas manifes.  
− Informasi hak cipta dan perizinan.  
− Informasi kontak untuk distributor atau pemrogram.  
− Bug yang diketahui.  
− Troubleshooting.  
− Kredit dan ucapan terima kasih.  
− Sebuah catatan perubahan/changelog (biasanya untuk pemrogram).  
− Bagian berita (biasanya untuk pengguna).