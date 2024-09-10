<h1>LAPORAN PRAKTIKUM SISTEM FILE</h1>
 <h2>PENDAHULUAN</h2>
 <h3>LATAR BELAKANG</h3>
<p>Sistem file adalah elemen fundamental dalam pengelolaan data pada sistem operasi komputer, berfungsi untuk menyimpan, mengorganisasikan, dan mengatur akses terhadap data di media penyimpanan seperti hard disk dan SSD. Sistem file menentukan bagaimana data disimpan secara fisik dan bagaimana file serta direktori diatur sehingga pengguna dapat dengan mudah mengakses dan memanipulasi informasi yang diperlukan. Dengan memahami cara sistem file bekerja, kita dapat memastikan bahwa data dikelola dengan efisien dan aman.</p>
<p>Praktikum ini dirancang untuk memberikan pemahaman praktis tentang manajemen file dan direktori di lingkungan sistem berbasis Unix/Linux. Fokus utama dari praktikum ini adalah pengelolaan izin akses file, yang merupakan aspek penting dalam menjaga keamanan data dan mengatur hak akses pengguna. Izin akses menentukan siapa yang dapat membaca, menulis, atau mengeksekusi file, sehingga pengaturan izin yang tepat sangat penting untuk melindungi data dari akses yang tidak sah dan memastikan bahwa kolaborasi dapat dilakukan dengan lancar. Selain itu, praktikum ini juga mencakup pembuatan dan pengaturan struktur direktori yang efisien. Struktur direktori yang baik memungkinkan pengorganisasian data yang lebih baik, memudahkan pencarian file, dan meningkatkan produktivitas. Selama praktikum, kami akan belajar bagaimana membuat dan mengelola direktori, serta menyalin, memindahkan, dan mengatur file di berbagai lokasi.</p>

Berdasarkan latar belakang diatas, maka tujuan penulisan laporan praktikum ini yaitu : <br/>
1.	Mengenal organisasi File di Linux<br/>
2.	Menciptakan dan manipulasi direktori<br/> 
3.	Mempelajari ijin akses (permission) dari file dan direktori <br/>
4.	Mengenal konsep Owner dan Group<br/>
5.	Mengerti konsep Link dan symbolic link<br/>
<h3>ALAT DAN BAHAN</h3>
1. Laptop <br/>
2. Virtual Box <br/>
3. Ubuntu 24.04 <br/>
<h3>DASAR TEORI</h3>
1. Sistem File <br>
Sistem file adalah cara sistem operasi mengatur data di media penyimpanan seperti hard disk atau SSD. Ini seperti sebuah buku yang membagi data ke dalam bab dan halaman, agar data bisa ditemukan dan diakses dengan mudah. Berbagai jenis sistem file, seperti FAT, NTFS, dan ext4, memiliki cara berbeda dalam menyimpan dan mengelola data, serta fitur tambahan yang masing-masing menawarkan.Linux<br>
2.	Izin Akses File <br/>
Izin akses file adalah aturan yang menentukan siapa yang bisa melihat, mengubah, atau menjalankan file. Di sistem operasi seperti Unix/Linux, izin ini dibagi untuk tiga kategori: pemilik file (user), grup pengguna (group), dan orang lain (others). Pemilik file biasanya memiliki kontrol penuh atas file tersebut, sementara grup dan orang lain hanya bisa memiliki hak akses tertentu. Ada tiga jenis izin: baca (read), tulis (write), dan eksekusi (execute). Hak baca memungkinkan pengguna melihat isi file, hak tulis memungkinkan mereka mengubahnya, dan hak eksekusi memungkinkan mereka menjalankan file jika itu adalah program.<br/>
3. Manajemen File <br/>
Manajemen file mencakup berbagai tindakan yang bisa dilakukan terhadap file, seperti membuat, menyalin, memindahkan, dan menghapusnya. Semua tindakan ini penting untuk menjaga data tetap terorganisir dan mudah diakses. Sistem file menyediakan alat dan perintah untuk melakukan semua operasi ini dengan efisien, membantu Anda mengelola data sehari-hari dengan lebih baik. <br/>
<h2>PEMBAHASAN</h2>
<h1>Langkah Langkah Praktikum</h1>

1.	Lihat peralatan I/O, character device, yang ada pada system komputer. <br/>
Jawab:<br/>
<img src = https://github.com/user-attachments/assets/320daed5-5e13-4b1a-8a29-b7121a9e6fb1 width=500 /> <br/>

2.	Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5.
Jawab:<br/>
<img src = https://github.com/user-attachments/assets/c9d6c490-b56d-43e5-9480-63c63d13e38c width=500 /> <br/>

3.	Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5.<br/>
Jawab:<br/>
<img src = https://github.com/user-attachments/assets/fa7220ab-d7ee-4c08-81fd-b3261ad686a3 width=500 /> <br/>
<img src = https://github.com/user-attachments/assets/981ffc62-8e53-4b6a-aed7-dcdadfbb75ce width=500 /> <br/>

4.	Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others dapat melakukan write.<br/>
Jawab:<br/>
<img src = https://github.com/user-attachments/assets/db8223fe-f6ff-41ee-b45f-c77443282b0e width=500 /><br/>

5.	Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read dan execute.<br/>
Jawab: <br/>
<img src = https://github.com/user-attachments/assets/44b24450-acd4-4003-a6ab-8e4284906249 width=500 /> <br/>

6.	Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat melakukan write, read dan execute. <br/>
Jawab: <br/>
<img src = https://github.com/user-attachments/assets/16c387b1-8619-42cf-b827-2c6fbefe7a4c width=500 /> <br/>

7.	Hapuslah direktori maret.<br/>
Jawab:<br/>
<img src = https://github.com/user-attachments/assets/b2ba0b29-7c53-46e2-88ab-01f3d43bea59 width=500 /> <br/>

8.	Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapat melakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori februari. <br/>
Jawab:<br/>
<img src = https://github.com/user-attachments/assets/4276720f-7358-497f-b3f1-923d70ca30e2 width=500 /> <br/>

9.	Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakan nilai default-nya ?<br/>
Jawab:<br/>

<img src = https://github.com/user-attachments/assets/490f4333-efb1-4bb4-94f6-689d087cbf72 width=500 /> <br/>
10.	Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah list perhatikan berapa link yang terjadi ?<br/>
Jawab:<br/>
<img src = https://github.com/user-attachments/assets/0a902602-0bcf-4dd1-bca8-8f4ff681324c width=500 /> <br/>

 


<h2>PENUTUP</h2>
<h3>KESIMPULAN</h3>
Praktikum ini memberikan pemahaman mendalam mengenai pengelolaan sistem file di lingkungan Unix/Linux, dengan penekanan pada manajemen file, struktur direktori, dan pengaturan izin akses. Dari praktikum ini, kita dapat menyimpulkan bahwa sistem file adalah komponen penting dalam mengatur dan menyimpan data di media penyimpanan, serta memahami cara kerja dan fungsinya sangat membantu dalam mengelola data secara efisien. Pengaturan izin akses file, yang menentukan siapa yang dapat membaca, menulis, atau menjalankan file, memainkan peran kunci dalam menjaga keamanan dan integritas data, serta memungkinkan kolaborasi yang aman. Struktur direktori yang baik memudahkan pengorganisasian dan pencarian file, sehingga mempermudah akses dan pemeliharaan data. Selain itu, penguasaan operasi dasar seperti pembuatan, penyalinan, dan penghapusan file adalah keterampilan penting dalam manajemen file sehari-hari. Secara keseluruhan, praktikum ini membekali kita dengan keterampilan praktis untuk mengelola sistem file secara efektif, baik dalam konteks akademik maupun profesional, dan menekankan pentingnya pengelolaan data yang aman dan efisien.<br/>
