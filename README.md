<h1 align="center">Selamat datang di repository Learnlynx!</h1>

![inipotonya png](https://github.com/Wiraapriliansyah/Learnlynx/assets/152155184/9d9ce6a4-93d1-47b8-b61a-7aeb7ce8f3c8)

<p></p>

<h4 align="center">Website e-learning yang membuat proses belajar mengajar menjadi lebih mudah dimana saja dan kapan saja<a href="https://codeigniter.com/" target="_blank"> Codeigniter</a>.
</h4>

<p></p>

<p align="center">
	<img src="https://img.shields.io/github/issues/syauqi/learnify?style=flat-square">
	<img src="https://img.shields.io/github/stars/syauqi/learnify?style=flat-square"> 
	<img src="https://img.shields.io/github/forks/syauqi/learnify?style=flat-square">
	<img src="https://img.shields.io/github/license/syauqi/learnify?style=flat-square">
	<img src="https://img.shields.io/github/followers/syauqi.svg?style=flat-square&label=followers">
</p>

<p align="center">
  <a href="#tentang">Tentang Project</a> •
  <a href="#fitur">Fitur</a> •
  <a href="#download">Download & Install</a> •
  <a href="#akun">Akun Default</a> •
  <a href="#lisensi">Lisensi</a>
</p>

<p></p>

<h2 id="tentang">🧑‍🏫 Tentang Learnlynx</h2>

Learnlynx dibuat agar para mahasiswa dan dosen dapat terus belajar dan mengajar dimana saja dan kapan saja, tanpa batasan ruang dan waktu.

<p></p>

<h2 id="fitur">🙌 Fitur Tersedia</h2>

- Autentikasi
  - Login mahasiswa, dosen dan admin
  - Daftar sebagai mahasiswa dan dosen
- Manajemen Data
  - Mahasiswa [akses video pembelajaran dan memberi tanggapan]
  - dosen [upload materi berdasarkan kelas dan mata kuliah]
  - Admin [mengatur data mahasiswa, dosen, dan materi]
- Diskusi dan Reaksi Dengan Integrasi Diskusi
- Ujian Online [segera hadir]

![image](https://github.com/Wiraapriliansyah/Learnlynx/assets/152155184/14192076-40b0-4e9d-baad-629132429b4d)

Entity relationship diagram (ERD) adalah diagram yang menggambarkan hubungan antara entitas dalam sistem. Pada gambar di atas terdapat enam entitas yang saling berhubungan, yaitu:
1. Admin
Admin memiliki atribut id_admin (atribut kunci), username, password, dan email. Admin dapat mengelola dosen, mahasiswa, kelas, dan materi. Ini berarti ada hubungan satu-ke-banyak antara admin dan entitas-entitas tersebut.
2. Dosen
Dosen memiliki atribut nip (atribut kunci), email, nama_dosen, nama_matkul, dan password. Dosen dapat mengajar dalam banyak kelas dan dapat mengunggah banyak materi. Ini berarti ada hubungan satu-ke-banyak antara dosen dan kelas, serta antara dosen dan materi. Dosen juga dapat diatur oleh admin. Ini berarti ada hubungan banyak-ke-satu antara dosen dan admin
3. Mahasiswa
Mahasiswa memiliki atribut nim (atribut_kunci), nama_mahasiswa, email, image, status_akun, dan tanggal_dibuat. Mahasiswa dapat terdaftar dalam banyak kelas dan dapat mengakses banyak materi. Ini berarti ada hubungan satu-ke-banyak antara mahasiswa dan kelas, serta antara mahasiswa dan materi. Mahasiswa juga dapat diatur oleh admin. Ini berarti ada hubungan banyak-ke-satu antara mahasiswa dan admin.
4. Token
Token memiliki atribut id_token (atribut kunci), email, token, tanggal_dibuat. Token dapat dikaitkan dengan mahasiswa untuk otentikasi. Ini berarti ada hubungan satu-ke-satu antara token dan mahasiswa.
5. Kelas
Kelas memiliki atribut id_kelas (atribut kunci), kelas, dan nama_mahasiswa. Kelas dapat memiliki banyak mahasiswa dan banyak materi. Ini berarti ada hubungan banyak-ke-satu antara kelas dan mahasiswa, serta antara kelas dan materi. Kelas juga dapat diatur oleh admin dan diajarkan oleh dosen. Ini berarti ada hubungan banyak-ke-satu antara kelas dan admin, serta antara kelas dan dosen.
6. Materi
Materi memiliki atribut id_materi, kelas, deskripsi, video, nama_matkul, dan nama dosen. Materi dapat diakses oleh banyak mahasiswa dan diajarkan dalam banyak kelas. Ini berarti ada hubungan banyak-ke-satu antara materi dan mahasiswa, serta antara materi dan kelas. Materi juga dapat diunggah oleh dosen dan diatur oleh admin. Ini berarti ada hubungan banyak-ke-satu antara materi dan dosen, serta antara materi dan admin.

<p></p>

<h2 id="akun">🔑 Daftar Akun Yang Tersedia</h2>

Berikut adalah beberapa akun yang dapat digunakan untuk masuk pertama kali, anda juga dapat membuat akun baru melalui halaman registrasi

| Role  | Email                    | Password | URL                                      |
| ----- | ------------------------ | -------- | ---------------------------------------- |
| Admin | admin@gmail.com          | admin    | http://localhost/Learnlynx/welcome/admin |
| Siswa | itadoriyuji@jujutsu.com  | 123456   | http://localhost/Learnlynx/welcome       |
| Guru  | ryomensukuna@jujutsu.com | 123456   | http://localhost/Learnlynx/welcome/guru  |

<p></p>

<h2 id="syarat">📑 Prasyarat yang Diperlukan</h2>

Berikut adalah daftar layanan dan aplikasi yang diperlukan untuk menjalankan aplikasi Learnlynx

- PHP 7, 8 & Web Server [XAMPP, LAMPP, MAMP]
- Web Browser [Chrome, Firefox, Safari & Opera]
- Internet [Karena menggunakan banyak CDN]
- Setting lanjutan PHP [max_upload & post_max di php.ini]

<p></p>

<h2 id="download">📖 Panduan Menjalankan & Install Aplikasi</h2>

Untuk menjalankan aplikasi atau web ini kamu harus install XAMPP dan mempunyai setidaknya satu browser yang terinstall di komputer anda.

```bash
# Clone repository ini atau download di
$ git clone https://github.com/syauqi/learnify.git

# Buat database
Buat database dengan nama "learnify" di DMBS [phpmyadmin, dll]

# Upload database
Arahkan folder ke learnify/database/Learnlynx.sql & upload ke dbms [phpmyadmin]

# Buka browser
http://localhost/Learnlynx/welcome

# Masukkan akun yang tersedia di atas untuk login sebagai admin, mahasiswa, atau dosen
```


<p></p>

<h2 id="kontribusi">🤝 Kontribusi</h2>

Contributions, issues and feature requests sangat saya apresiasi karena aplikasi ini jauh dari kata sempurna. Jangan ragu untuk pull request dan membuat perubahan pada project ini.

Berhubung Project ini saya selesaikan sendiri, namun banyak fitur dan banyak hal yang bisa diperbaiki maka bantuan kalian sangat saya apresiasi.

<p></p>

<h2 id="lisensi">🔖 Lisensi</h2>

- Copyright © 2023 Wira Apriliansyah Saputra
- Learnlynx adalah aplikasi web open-source yang berlisensi dibawah lisensi MIT
- Referensi https://github.com/syauqi/learnify

---

**<p align="center">Made by Wira Apriliansyah Saputra</p>**
