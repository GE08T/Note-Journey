
Tanggal Pembuatan : 23-06-202520:14

Status : ~~finished~~

Tag : [[VSGA]], [[Web Development]]

#### Menerapkan coding-guidelines dan best practices dalam penulisan program (kode sumber)

##### Coding-standard HTML
Pastikan kode html sesuai dengan HTML 5 Best Practices, jangan lupakan indentasi gunakan prettier

##### Coding-standard untuk CSS
**Format CSS**
- Semua dokumen CSS harus menggunakan dua spasi untuk indentasi dan file tidak boleh memiliki dua spasi tambahan (whitespace).
- Gunakan tanda kutip ganda.
- Gunakan notasi steno hanya jika diperlukan.
- Beri spasi setelah: dalam deklarasi properti.
- Letakkan spasi sebelum {dalam deklarasi aturan.
- Gunakan kode warna hex # 000 kecuali menggunakan rgba ().
- Selalu berikan properti fallback untuk browser lama.
- Gunakan satu baris per deklarasi properti.
- Selalu ikuti aturan dengan satu baris spasi.
- Selalu mengutip konten url () dan @import ().
- Jangan membuat indentasi blok.

##### Coding Standard untuk PHP
pastikan dalam penggunaan tag benar dan baik ataupun penamaan variabel merepresentasi apa yang dilakukan variabel tersebut

**Function**
● Nama fungsi harus menggunakan huruf kecil dan kata-kata harus dipisahkan oleh garis bawah  
   Contoh: function welcome_message() {  
● Awalan fungsi HARUS dimulai dengan kata kerja  
   Contoh: get_, add_, update_, delete_, convert_, dll  
● Pemanggilan fungsi tidak boleh menggunakan spasi antara nama fungsi dan tanda kurung terbuka  
   Contoh: func();  
● Argumen didalam fungsi harus dituliskan sbb:  
● Tidak boleh menggunakan spasi sebelum tanda koma.  
● Harus menggunakan spasi setelah tanda koma.  
● Boleh menggunakan baris baru untuk argument yang Panjang.  
● Setiap argument harus dituliskan di baris yang berbeda  
● Harus menggunakan satu kali indentasi untuk argument dibawahnya  
● Harus diurutkan dari yang paling dibutuhkan sampai argument pilihan.  
● Harus diurutkan berdasarkan argumen yang paling penting ke argument yang tidak begitu penting.  
● Harus menggunakan standar deskriptif.  
● HARUS menyertakan petunjuk jenis.  
   misalnya func($arg1, $arg2 = 'asc', $arg3 = 100);  
● Deklarasi fungsi HARUS didokumentasikan menggunakan pedoman  
       - phpDocumentor dan HARUS meliputi:  
       - Deskripsi Singkat  
       - Deskripsi Panjang, jika perlu  
       - @access: private atau protected (diasumsikan public)  
       - @penulis: nama penulis  
       - @global: menggunakan fungsi variabel global, jika ada  
       - @param: Parameter dengan tipe data, nama variabel, dan deskripsi  
       - @return: Kembalikan tipe data, jika ada

##### Best-Practice untuk PHP

**Inisialisasi variable**
● Inisialisasi variable harus dilakukan pertama kali sebelum penggunaan variable tersebut

**Inisialisasi/ Urutan deklarasi variable, method dan properties**
● HARUS diawali dengan global, ikuti dengan konstanta, dan diakhiri dengan variabel lokal  
● HARUS diawali dengan properti kemudian diikuti dengan method dalam class  
● HARUS diawali dengan public, diikuti protected, dan diakhiri dengan private method dalam class 
● HARUS sesuai dengan abjad dalam kelompoknya

**Penanganan Galat/Error**
● Penanganan error adalah proses menangkap kesalahan pada program untuk diambil tindakan yang sesuai.  
● Metode Penanganan Error  
    - Menggunakan Function "die()"  
    - Menulis function Penanganan Error sendiri  
    - Error reporting
● Program akan terhenti ketika memanggil function die(); dan menampilkan pesan yang dapat dipahami oleh pengguna

**Menulis function Penanganan Error sendiri**
● Fungsi yang dibuat harus mampu menangani minimal dua parameter (tingkat kesalahan dan pesan kesalahan) tetapi dapat menerima hingga lima parameter  
(opsional: file, nomor baris, dan konteks kesalahan):
![[Pasted image 20250623203124.png|400]]
● Level Kesalahan:
![[Pasted image 20250623203209.png|]]

**Penanganan pengecualian (exception)**
● Pengecualian digunakan untuk mengubah alur program yg normal jika terjadi kesalahan (error) tertentu. Kondisi tersebut disebut pengecualian.  
● Pada dasarnya yang terjadi saat exception dipicu adalah:  
- Keadaan kode yang paling baru (sebelum terjadi kesalahan) disimpan  
- Eksekusi kode akan beralih ke fungsi handler exception (custom) yang telah ditentukan  
- Bergantung pada situasinya, handler kemudian dapat melanjutkan eksekusi dari status kode yang disimpan, mengakhiri eksekusi program atau melanjutkan program dari lokasi yang berbeda dalam kode.  

**Penggunaan Exception dasar**
● Penulisan Exception yang standard harus mengandung:  
- try - Fungsi yang menggunakan exception harus berada di dalam blok “try". Jika exception tidak terpicu, kode akan dilanjutkan seperti biasa. Namun jika exception terpicu, exception akan di-“throw“.  
- throw - Ini adalah bagaimana Anda memicu exception. Setiap “throw" harus memiliki setidaknya satu “catch“.  
- catch - Blok "catch" mengambil exception dan membuat objek yang berisi informasi dari execption.

**Error Reporting**
● Fungsi error_reporting () menentukan kesalahan mana yang dilaporkan.  
● PHP memiliki banyak level kesalahan, dan menggunakan fungsi ini menetapkan level kesalahan tersebut untuk kode program yang sedang dijalankan.

**Kinerja Situs Web**
● Ketika berbicara tentang kinerja aplikasi web, kita berbicara tentang kinerja web atau kinerja runtime.  
● Kinerja web sebagai ukuran waktu mulai dari saat pengguna akhir meminta konten hingga kapan konten itu tersedia di perangkat pengguna.  
● Kinerja runtime sebagai indikasi seberapa responsif aplikasi terhadap input pengguna saat runtime.

##### Menggunakan ukuran performansi dalam menuliskan kode sumber
Mengukur Kinerja Program (kecepatan)
Waktu Eksekusi = Waktu Berakhir – Waktu Mulai
![[Pasted image 20250623203533.png|350]]
##### Mengukur Kinerja Program (penggunaan memory)
![[Pasted image 20250623203558.png|350]]

##### Menulis kode PHP dengan Efisien
● Menggunakan Fungsi bawaan PHP  
   Menggunakan fungsi bawaan PHP lebih cepat dibanding menulis fungsi sendiri.  
   Referensi fungsi bawaan PHP dapat dilihat di manual PHP [https://www.php.net/manual/en/funcref.php](https://www.php.net/manual/en/funcref.php)  
● Membuat Kelas hanya jika diperlukan  
   Kelas dan method dibuat jika memang benar-benar diperlukan (digunakan kembali di banyak kode).  
● Menutup Koneksi  
   Menutup koneksi basisdata setelah tidak dibutuhkan akan menghemat memory.  
● Menggunakan petik tunggal  
  Ketika menggunakan string, penggunaan petik tunggal ( ‘ ‘ ) lebih cepat dari pada petik ganda ( ” ” ). Petik ganda akan memeriksa keberadaan variabel di dalamnya, sehingga butuh waktu lebih lama
  ● Mengurangi perhitungan yang tidak perlu 
  Menghitung dan memberikan nilai ke variabel di awal, lebih cepat dari pada menghitungnya beberapa kali dimana perhitungan tersebut diperlukan.
  ● Menggunakan function isset()
  Gunakan isset() jika memungkinkan untuk memeriksa lebih besar dari 0. Hindari menggunakan count( ), strlen( ), sizeof( ).
  ● Menggunakan Swith Case dibanding If
Menggunakan pernyataan case lebih efisien dibandingkan struktur if/else untuk mengerjakan pekerjaan yang sama.

#### Mengimplementasikan Kemudahan Interaksi
 kita perlu memperhatikan juga kemudahan aplikasi ketika digunakan oleh pengguna. Aplikasi yang dibuat harus dipastikan sesuai dengan panduan desain Antarmuka Pengguna (User Interface).
 
##### 10 Panduan desain antarmuka pengguna Nielsen dan Molich's
1. Visibilitas status sistem.
	Pengguna harus selalu diberitahu tentang status proses yang terjadi. Pemberitahuan harus mudah dimengerti, mudah terlihat di layar, dan ditampilkan dalam waktu yang wajar.
	
 2. Aplikasi sesuai dengan dunia-nyata
	 Sistem harus menggunakan bahasa, kata-kata, frasa dan konsep yang familiar dengan pengguna. Menyajikan informasi dalam urutan logis dan mendukung ekspektasi pengguna yang berasal dari pengalaman mereka di dunia nyata akan membuat sistem lebih mudah digunakan.
	 
 3. Kontrol dan Kebebasan Pengguna
	 Tawarkan ruang digital kepada pengguna agar memungkinkan langkah mundur, termasuk membatalkan dan mengulangi tindakan sebelumnya.
	 
  4. Konsistensi dan Standar
	  Elemen grafis dan terminologi dipertahankan di seluruh platform yang sama. Misalnya, ikon yang mewakili satu kategori atau konsep tidak boleh mewakili konsep yang berbeda ketika digunakan pada layar yang berbeda.
	  
5. Pencegahan Kesalahan
	Sistem dirancang agar potensi kesalahan dijaga seminimal mungkin. Pengguna tidak suka dipanggil untuk mendeteksi dan memperbaiki masalah, yang kadang-kadang berada di luar tingkat keahlian mereka. dapat dilakukan dengna menghilangkan atau menandai tindakan yang dapat menyebabkan kesalahan.
	
 6. Mengenali daripada mengingat
	 Minimalkan beban memori pengguna. Buat objek, tindakan, dan opsi terlihat. Pengguna tidak harus mengingat informasi dari satu bagian dialog ke bagian lainnya. Petunjuk penggunaan sistem harus terlihat atau mudah diambil kapan pun diperlukan.
	 
 7. Fleksibilitas dan efisiensi penggunaan
	 Interaksi yang lebih sedikit yang memungkinkan navigasi lebih cepat.  Sehingga sistem dapat melayani pengguna yang tidak berpengalaman maupun yang berpengalaman.  Izinkan pengguna untuk menyesuaikan tindakan yang sering dilakukan.  Dapat menggunakan singkatan, tombol fungsi, perintah tersembunyi dan fasilitas makro.
	
 8. Desain estetis dan minimalis
	 Interaksi/infor dengan pengguna dijaga agar tetap minimalis dengan tetap memperhatikan keindahan dan kegunaan , Tampilan harus dikurangi menjadi hanya komponen yang diperlukan untuk tugas saat ini, sehingga memberikan cara yang jelas dan tidak ambigu untuk menavigasi ke konten lain.
	 
 9. Bantu pengguna mengenali, mendiagnosis, dan memulihkan dari kesalahan
10. Bantuan dan Dokumentasi
	 Meskipun lebih baik jika sistem dapat digunakan tanpa dokumentasi, mungkin perlu memberikan bantuan dan dokumentasi.   Setiap informasi seperti itu harus mudah dicari, difokuskan pada aktifitas pengguna, daftar langkah konkret yang harus dilakukan, dan tidak terlalu besar.
	 
#### Menggunakan ukuran performansi dalam menuliskan kode sumber
(kosong)

#### Menggunakan tipe data dan control program
membahas tentang penggunaan variabel dan tipe data yang baik dan benar

#### Tips
Ketrampilan yang diperlukan dalam menulis kode dengan prinsip sesuai guidelines dan best practices

1. Menerapkan coding- guidelines dan best practices dalam penulisan program (kode sumber)  
2. Menggunakan ukuran performansi dalam menuliskan kode sumber  
3. Menggunakan tipe data dan control program
