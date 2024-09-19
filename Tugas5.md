## Tugas 5 Sistem Operasi ##

### 1. Lihat daftar secara lengkap pada direktori aktif, belokkan tampilan standard output ke file baru. ###
Untuk menampilkan daftar direktori yang sedang aktif, gunakan perintah `$ ls`, sedangkan untuk membelokkan output standar ke file baru, gunakan tanda `>`.

<img width="411" alt="Screenshot 2024-09-19 084400" src="https://github.com/user-attachments/assets/2173b2f6-5ff5-45eb-b03c-7a06be6aa8e8">

### 2. Lihat daftar secara lengkap pada direktori /etc/passwd, belokkan tampilan standard output ke file baru tanpa menghapus file baru sebelumnya ###
Untuk melihat daftar lengkap dari direktori `/etc/passwd`, gunakan perintah `$ ls`, sedangkan untuk mengalihkan output standar ke file baru tanpa menghapus file baru sebelumnya, gunakan tanda `>>`.

<img width="413" alt="Screenshot 2024-09-19 084532" src="https://github.com/user-attachments/assets/a2ac94ce-3caa-4143-84b7-a75943a2d0cd">

### 3. Urutkan file baru dengan cara membelokkan standard input ###
Untuk mengurutkan file, gunakan perintah `$ sort`, sedangkan untuk membelokkan standard input, gunakan tanda `<`.

 <img width="407" alt="Screenshot 2024-09-19 084618" src="https://github.com/user-attachments/assets/f7d56646-9c07-4be7-b20d-07ebc1267b6d">

### 4. Urutkan file baru dengan cara membelokkan standard input dan standard output ke file baru.urut ###
Untuk mengurutkan file, gunakan perintah `$ sort`. Untuk mengalihkan input standar, gunakan tanda `<`, dan untuk mengalihkan output standar ke file, gunakan tanda `>`. Pembelokkan input dan output standar dapat dikombinasikan, namun nama file yang digunakan untuk input dan output tidak boleh sama.

<img width="402" alt="Screenshot 2024-09-19 084924" src="https://github.com/user-attachments/assets/98e91f4e-5920-44fb-85e8-0d63ca40ad43">

### 5. Buatlah direktori latihan6 sebanyak 2kali dan belokkan standard error ke file rmdirerror.txt. ###
Gunakan perintah `$ mkdir` untuk membuat direktori baru. Ketika mencoba membuat direktori yang sama lagi, akan muncul pesan kesalahan. Pesan kesalahan tersebut dapat dibelokkan ke file menggunakan tanda `2>`.

<img width="410" alt="Screenshot 2024-09-19 085224" src="https://github.com/user-attachments/assets/d72a9740-f269-4ec6-87e6-96f74be9ee4d">

### 6. Urutkan file berikut dengan menggunakan notasi here document : ###
#### sort <<@@@ ####
#### Jakarta ####
#### Bandung ####
#### Surabaya ####
#### Padang ####
#### Palembang ####
#### Lampung ####
#### @@@ ####
Pertama, buat notasi *here document* yang dialihkan ke sebuah file, lalu isi dokumen tersebut. Setelah diisi dan diakhiri, isinya akan tersimpan ke file yang dialihkan. File tersebut kemudian dapat diurutkan menggunakan perintah `$ sort`.

<img width="410" alt="Screenshot 2024-09-19 085422" src="https://github.com/user-attachments/assets/38fe441f-025a-4b2a-8299-fd36d5eebaed">

### 7. Hitung jumlah baris, kata, dan karakter dari file.urut dengan menggunakan filter dan tambahkan data tersebut ke file baru. ###
Untuk mendapatkan jumlah baris, kata, dan karakter (secara berurutan) dari sebuah file, gunakan perintah `wc` yang dipadukan dengan perintah `cat` menggunakan pipa. Hasilnya kemudian dapat ditambahkan ke file menggunakan tanda `>>`.

<img width="404" alt="Screenshot 2024-09-19 091107" src="https://github.com/user-attachments/assets/7ad648c0-5e40-4a2c-97c9-a2ce8fa8f849">

### 8. Gunakan perintah di bawah ini dan perhatikan hasilnya : ###
#### cat /etc/passwd | sort | pr -n | grep | tty03 ####
Menampilkan isi /etc/passwd, mengurutkannya, menomori barisnya, dan mencari baris yang mengandung tty03.
#### find /etc -print | head ####
Menampilkan 10 baris pertama dari daftar file dan direktori di dalam /etc.
#### head /etc/passwd | tail -5 | sort
Menampilkan 5 baris terakhir dari 10 baris pertama file /etc/passwd, kemudian mengurutkannya.

<img width="410" alt="Screenshot 2024-09-19 091458" src="https://github.com/user-attachments/assets/8f19d666-ce25-4f91-8604-09018f03c62a">

### 9. Gunakan perintah berikut dan perhatikan hasilnya : ### 
#### who | cat | cat | sort | pr | head | cat | tail ####
Untuk menampilkan pengguna yang sedang login, gunakan perintah `who`, lalu urutkan hasilnya dengan `sort`. Setelah itu, format output sesuai kebutuhan, dan gunakan perintah untuk menampilkan baris pertama `head` dan terakhir `tail` dari hasil tersebut.

<img width="392" alt="Screenshot 2024-09-19 091612" src="https://github.com/user-attachments/assets/d656ad71-8113-4eb0-9734-b81c80496d48">
