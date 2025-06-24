
Tanggal Pembuatan : 23-06-2025 19:24

Status : ~~finished~~

Tag : [[VSGA]], [[Web Development]]

#### Mekanisme Server
1. Request > http > server > http > client 
2. Local = xampp 

#### Mekanisme HTML 
Model kerja HTML diawali dengan permintaan suatu halaman web oleh browser. Berdasarkan URL _(Uniform Resource Locator)_, browser mendapatkan alamat dari web server, mengindentifikasi halaman yang dikehendaki, dan menyampaikan segala informasi yang dibutuhkan oleh web server. Selanjutnya, web server akan mencarikan berkas yang diminta dan memberikan isinya ke browser. Browser yang mendapatkan isinya segera melakukan proses penerjemahan kode HTML dan menampilkannya ke layar pengguna.

#### Mekanisme PHP
Prinsipnya adalah ketika berkas PHP yang diminta didapatkan oleh web server, isinya segera dikirimkan ke mesin PHP yang memproses dan memberikan hasilnya (berupa kode HTML) ke web server. Selanjutnya, web server menyampaikan ke klien.  

Salah satu kelebihan dari PHP adalah mampu berkomunikasi dengan berbagai database yang terkenal. Menampilkan data yang bersifat dinamis yang diambil dari database merupakan hal yang mudah untuk diimplementasikan. Beberapa database tersebut antara lain MSQL, MySQL, Oracle, Postgre SQL, dan Sybase.

#### Tag Dasar PHP, Running 
***SKIP*  already know it**

#### Xampp 
XAMPP ialah perangkat lunak bebas yang mendukung banyak sistem operasi, merupakan campuran dari beberapa program. Yang mempunyai fungsi sebagai server yang berdiri sendiri (localhost).

##### Komponen XAMPP
• Apache versi 2.4.39 adalah aplikasi web server default;
• MariaDB versi 10.1.38 adalah sistem manajemen database;
• PHP versi 7.3.4 adalah server side scripting untuk membuat aplikasi berbasis web;
• phpMyAdmin versi 4.8.5 adalah tool untuk menggunakan MySQL berbasis web;
• OpenSSL versi 1.1.0g adalah implementasi open-source dari dua protokol keamanan populer, yaitu SSL dan TSL ;
• XAMPP Control Panel versi 3.2.3 adalah kontrol panel sederhana untuk mengatur komponen berbeda pada XAMPP;

##### Eksekusi kode dan Database
kode :  http://localhost/nama_project
database : http://phpmyadmin.net/

##### Debugging dan Executable
Debugging merupakan serangkaian langkah dan aktivitas yang melibatkan identifikasi, analisis, serta perbaikan kesalahan atau bug yang mungkin muncul dalam struktur dan eksekusi suatu kode program.

Executable tahapan yang melibatkan konversi kode sumber suatu perangkat lunak ke dalam bentuk yang dapat dijalankan secara mandiri, tanpa memerlukan interpretasi atau terjemahan langsung oleh Bahasa pemrograman yang digunakan. ex : file .exe .msi

#### Memastikan Script sesuai dengan Scenario 
Dilakukan pengujian untuk script agar memastikan script tidak ditemukan kesalahan.

Secara umum dari proses testing adalah melakukan verifikasi, validasi, dan mendeteksi terjadinya error pada aplikasi tersebut. Dari ketiga hal tersebut diharapkan dapat menemukan masalah – masalah atau kesalahan dan dari hasil penemuan tersebut dapat dilakukan suatu pembenahan.
##### Prinsip Pengujian Pelatihan
● Harus bisa dilacak hingga sampai ke kebutuhan customer.
● Harus direncanakan sejak model dibuat.
● Prinsip Pareto: 80% error uncovered.
● Dari lingkup kecil menuju yang besar.
● Tidak bisa semua kemungkinan diuji.
● Dilakukan oleh pihak ketiga yang independen.

##### Testability
Menguji apakah script tersebut mudah untuk diuji.
Karakteristiknya:
- Operability: mudah digunakan.
- Observability: mudah diamati.
- Controlability: mudah dikendalikan.
- Decomposability: mudah diuraikan.
- Simplicity: lingkup kecil, semakin mudah diuji.
- Stability: jarang berubah.
- Understandability: mudah dipahami.

##### Desain Testing
 Black box testing
- Memastikan fungsional Software berjalan.
- Kesesuaian input dengan output.
- Tidak memperhatikan proses logic internal.
Ex :
Equivalence Partitioning : Input NIM dalam Sistem Akademik
- Jika dikosongi?
- Jika diisi dengan format yang salah?
- Jika diisi dengan NIM yang benar?
Analisa Nilai Batas : ambang batas pada jam masuk tidak boleh lebih dari jam pulang 

White box testing
- Pengamatan detail prosedur.
- Mengamati sampai level percabangan kondisi dan perulangan.
Ex : 
logical path (jalur logika) perangkat lunak

#### Mengidentifikasi hasil eksekusi
##### Mengapa Menggunakan Source Code ?
agar dapat diuji secara : Structural Testing process, Program Logic-driven Testing, Design-based Testing, Examines the internal structure of program

##### Keuntungan Menggunakan Source Code
Menghasilkan program yang benar dan sempurna 100%, karena:
● Mengerjakan seluruh keputusan logika
● Mengerjakan seluruh loop (sesuai batas)
● Menjamin seluruh jalur independen dalam modul dikerjakan minimal 1x
● Mengerjakan seluruh data internal yang menjamin validitas dengan syarat:
- Mendefinisikan semua logical path
- Membangun kasus untuk pengujian – Mengevaluasi hasilnya
- Menguji secara menyeluruh

##### Jenis Kesalahan 
Internal Error : error pada kode program
Internal error dapat dicegah dengan pemrograman yang lebih hati-hati
ex : Parse Error/ Syntax Error, Fatal Error, Warning Error, Notice

Eksternal Error: error pada interaksi dengan hal lain diluar kode program. Eksternal error berkaitan dengan gagal membuka file/database, tidak terkoneksi dengan jaringan, tidak dapat membuka module/file php, dll.
ex : 
● 1xx : Informasi, yang menunjukkan bahwa Permintaan dipahami, melanjutkan proses. Kode ini hanya digunakan untuk status saja.
● 2xx : Sukses, Pada kode ini, server memberikan status suksesnya diterima, dipahami, disetujui, dan diprose.
● 3xx : Pengalihan
● 4xx : Kesalahan Klien, Pada kode ini, klien memberikan status kesalahan dalam memproses permintaan.
● 5xx : Kesalahan Server


##### Jenis Kesalahan Umum Pada Client
1. Error 404 (Not Found)/Broken Link
2. Error 403 (Forbidden)/Broken Link
3. Error 500 (Internal Server Error)
4. Error 503 (Service Unavailable)
5. Error 504 (Gateway Time-out)

#####  Kesalahan tidak dapat diakses setelah Hosting (Parse Error)
hal yang harus diperhatikan dalam menghosting ke server :  
1. Setting DNS  
2. File index  
3. Nama domain  
4. Koneksi Internet  
5. IP terblokir  
6. Komputer terserang ARP Spoofing/trojan/virus  
7. Upload file  
8. Pengaturan file php.ini  
9. Pengaturan database

Beberapa kesalahan yang Sering terjadi : 
- Kesalahan Setting DNS
- File Index : tidak ada, isinya kosong
- Koneksi Internet 
- IP Terblokir firewall
	Penyebab nya : 
	- Berkali-kali salah saat login cpanel/webmail/ftp/ssh/pop3/imap  
	- Terlalu sering me-refresh browser  
	- Melakukan spam  
	- Hacking  
	- DOS attack  
	- Port scan
* Komputer terserang virus
* Upload File yang tidak sempurna
* Pengaturan file php. Ini
* Pengaturan Database

 Keterampilan yang diperlukan dalam menerapkan perintah eksekusi pemrograman berbasis teks, grafik, dan multimedia

1. Mengidentifikasi mekanisme running atau eksekusi source code  
2. Mengeksekusi source code  
3. Mengidentifikasi hasil eksekusi