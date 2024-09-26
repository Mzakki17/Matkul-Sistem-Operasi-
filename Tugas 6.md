## TUGAS 6 SISTEM OPERASI : JOB CONTROL ##

#### 1. Eksekusi seluruh profile yang ada : ####
  #### a.  Edit file profile /etc/profile dan tampilkan pesan sebagai berikut : ####
  Echo “Profile dari /etc/profile” 

<img width="346" alt="Screenshot 2024-09-26 070647" src="https://github.com/user-attachments/assets/a789d891-1646-47a9-a58e-6447c9d64ca7">

  #### b. Asumsikan nama anda stD02001, maka edit semua profile yang ada yaitu :
   /home/stD02001/.bash_profile  
   /home/. stD02001/.bash_login  
   /home/mahasiswa/.profile  
   /home/mahasiswa/.bashrc  

   <img width="413" alt="Screenshot 2024-09-26 071557" src="https://github.com/user-attachments/assets/671d4ea8-7361-44c1-a148-6df10c772f20">

  #### c. Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile :  
  ##### echo “Profile dari .bash_profile”  
  ##### Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan.  

<img width="412" alt="Screenshot 2024-09-26 071701" src="https://github.com/user-attachments/assets/894a8613-f190-401c-b7d2-3820344c9ed0">
<img width="407" alt="Screenshot 2024-09-26 071343" src="https://github.com/user-attachments/assets/5a91055f-a092-42f6-9b0c-25d87fda64e4">
<img width="417" alt="Screenshot 2024-09-26 072231" src="https://github.com/user-attachments/assets/6a241f73-4b3e-4d35-b90b-3571b3a6f4b3">
<img width="412" alt="Screenshot 2024-09-26 072138" src="https://github.com/user-attachments/assets/583585a5-a26f-44cf-93dd-dbca976e6790">

  #### c.  Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:  

<img width="410" alt="Screenshot 2024-09-26 072414" src="https://github.com/user-attachments/assets/d2da2b31-e039-4f2f-9ddc-4af018e6185c">

  #### Jelaskan perbedaan kedua utilitas tersebut. 
  ##### 1. su mahasiswa :
  Perintah ini menjalankan su untuk beralih ke user mahasiswa. Saat menggunakan perintah ini tanpa opsi -, lingkungan (environment) dari user saat ini tetap dipertahankan. Artinya, hanya identitas pengguna yang berubah, tetapi variabel lingkungan seperti PATH tidak akan berubah. Jadi, variabel lingkungan dan direktori kerja yang sedang aktif tetap sama seperti sebelumnya.
  ##### 2. su-mahasiswa : 
  Perintah ini menggunakan opsi - yang dikenal sebagai login shell. Opsi ini melakukan login penuh sebagai user mahasiswa, sehingga environment yang dimuat adalah environment milik mahasiswa secara lengkap. Ini termasuk mengubah direktori kerja ke home directory user mahasiswa dan memuat variabel lingkungan seperti yang didefinisikan dalam shell milik mahasiswa. Jadi, ini seperti memulai sesi baru sebagai user mahasiswa.

#### 2. Prompt String (PS1)
  #### a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell 

<img width="416" alt="Screenshot 2024-09-26 073017" src="https://github.com/user-attachments/assets/adf63b0b-1dda-4c65-8b2e-e75e7804a8f4">
<img width="411" alt="Screenshot 2024-09-26 072951" src="https://github.com/user-attachments/assets/67ec9219-da5b-4afd-9996-7ab79001e354">

  #### b. Eksperimen hasil PS1.

<img width="418" alt="Screenshot 2024-09-26 074942" src="https://github.com/user-attachments/assets/98053a03-f07f-41a6-8f20-7086ac7d4f68">

#### 3. Logout
  #### a. Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout 

<img width="398" alt="Screenshot 2024-09-26 075758" src="https://github.com/user-attachments/assets/43647f8f-7e5d-41bb-b33b-62fbba2db7c5">
<img width="406" alt="Screenshot 2024-09-26 075223" src="https://github.com/user-attachments/assets/e92a6337-b669-4cfd-a566-fa4e10bd77f5">

#### 4. Bash Script
  #### a.  Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing : 
    p1.sh  
    #! /bin/bash  
    echo “Program p1”  
    ls –l  
    p2.sh  
    #! /bin/bash  
    echo “Program p2”  
    who  
    p3.sh  
    #! /bin/bash  
    echo “Program p3”  
    ps x 

<img width="413" alt="Screenshot 2024-09-26 075818" src="https://github.com/user-attachments/assets/4101538b-7be9-4832-8d11-000bba810241">
<img width="411" alt="Screenshot 2024-09-26 075425" src="https://github.com/user-attachments/assets/3990c136-deff-4569-b1e2-29c85fe5d66f">
<img width="407" alt="Screenshot 2024-09-26 075526" src="https://github.com/user-attachments/assets/204590f7-44f7-44a6-a922-a36d0760bb24">
<img width="414" alt="Screenshot 2024-09-26 075714" src="https://github.com/user-attachments/assets/931f7632-9c68-4145-a3da-83f9ad08ddb9">

  #### b. Jalankan script tersebut
  
<img width="611" alt="Screenshot 2024-09-26 080115" src="https://github.com/user-attachments/assets/d94f5854-3877-4c80-b674-4590ee81be17">
<img width="596" alt="Screenshot 2024-09-26 080154" src="https://github.com/user-attachments/assets/ae71799f-88b7-475c-81cc-0df8f5b1cd57">
<img width="599" alt="Screenshot 2024-09-26 080227" src="https://github.com/user-attachments/assets/947782db-e72b-4ddf-b42a-e6e8941446ef">
<img width="626" alt="Screenshot 2024-09-26 080252" src="https://github.com/user-attachments/assets/ee952d54-8673-4469-80c5-51d20c980a0d">
<img width="572" alt="Screenshot 2024-09-26 080641" src="https://github.com/user-attachments/assets/c792997f-952e-432f-935f-ee8898c35eb2">
<img width="611" alt="Screenshot 2024-09-26 080857" src="https://github.com/user-attachments/assets/7d2c5106-7582-4969-bf9b-544d2c53eefd">
<img width="612" alt="Screenshot 2024-09-26 081123" src="https://github.com/user-attachments/assets/4ef8e5c6-047f-4e47-b6e6-703bde0ff857">

#### 5. Jobs
  #### a.  Buat shell-script yang melakukan loop dengan nama pwaktu.sh, setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil. 

<img width="602" alt="Screenshot 2024-09-26 081654" src="https://github.com/user-attachments/assets/28d25e7d-d8fe-4fd6-8cdb-742c65deda53">
<img width="608" alt="Screenshot 2024-09-26 081301" src="https://github.com/user-attachments/assets/9dfad530-d350-4bbf-8c01-0b924f5f6f28">

  #### b.  Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut : 

<img width="554" alt="Screenshot 2024-09-26 082410" src="https://github.com/user-attachments/assets/a1b864c8-44b0-4e68-96e2-a22c9d086ef9">

  #### c. Jadikan program find sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background :
  
<img width="605" alt="Screenshot 2024-09-26 082607" src="https://github.com/user-attachments/assets/0ec48d21-c967-466e-b8a9-7c6eac1c1dbd">

  #### d. Stop program backgroung dengan utilitas kill : 
  
<img width="614" alt="Screenshot 2024-09-26 082701" src="https://github.com/user-attachments/assets/e9eb196a-41f0-4983-8a5c-5c6b846de08a">
<img width="610" alt="Screenshot 2024-09-26 082821" src="https://github.com/user-attachments/assets/85faa369-4b0a-4c1e-be00-ce1fe5b933ef">

#### 6. History :
  #### a. Ganti nillai HISTSIZE dari 1000 menjadi 20 :

<img width="611" alt="Screenshot 2024-09-26 082917" src="https://github.com/user-attachments/assets/84e743cc-503c-42cd-80c1-50b25c1e8061">

  #### b. Gunakan fasilitas history dengan mengoreksi instruksi baris ke-5 dari instruksi yang terakhir di lakukan :
  
<img width="604" alt="Screenshot 2024-09-26 083313" src="https://github.com/user-attachments/assets/87069849-494b-475a-9067-b22413c7159a">

  #### c. Ulangi instruksi yang terakhir.  Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer 
  
  <img width="610" alt="Screenshot 2024-09-26 083404" src="https://github.com/user-attachments/assets/34c0b450-3468-44ae-be36-2f8e637f5d90">

  #### d. Ulangi instruksi pada history bufer nomor 150 

<img width="575" alt="Screenshot 2024-09-26 083529" src="https://github.com/user-attachments/assets/7dce3f73-1902-461f-bece-03f89ddbba30">

  karena history nomor 150 tidak ada jadi diganti history nomor 39
  #### e. Ulangi instruksi dengan prefix “ls”   

<img width="519" alt="Screenshot 2024-09-26 083647" src="https://github.com/user-attachments/assets/ec9e9988-252b-42ba-ac89-190140473cda">
