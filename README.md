# PENI-ILHAMI_0901118232810.Tugas3-Sistem-Operasi
  <div align="center">

## Tugas Praktikum 3 Sistem File (File System)

*Dosen Pengampu:*\
Ahmad Heryanto, M. T.\
Adi Hermansyah, M. T.\
Sutarno, M.T.\
Iman Saladin B. Azhar, S. Kom., M. M.SI.\
Dr. Ahmad Zarkarsi, M. T.

<img src="https://github.com/user-attachments/assets/b086809c-d41c-4331-a4f6-93500d076a9c" alt="Alt Text" width="400">

<br>
<br>

*Disusun Oleh:*\
NAMA        : PENI ILHAMI\
NIM         : 09011182328101\
KELAS       : SK3B

<br>
<br>

*PRODI SISTEM KOMPUTER*  
*FAKULTAS ILMU KOMPUTER*  
*UNIVERSITAS SRIWIJAYA*  
*2024*
<br>
<br>

</div>

### TUGAS

<div align="justify">

1. Lihat peralatan I/O, character device, yang ada pada system komputer. 

  <img widthy="500" alt="Screenshot from 2024-09-11 01-04-36" src="https://github.com/user-attachments/assets/fa8f6fc4-f6be-47ce-a93f-f32b55e453cd">

  <img widthy="500" alt="Screenshot from 2024-09-11 01-15-22" src="https://github.com/user-attachments/assets/109289de-6de0-400c-8181-bacaed9d0ba9">


2. Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5. 

  <img widthy="500" alt="Screenshot from 2024-09-11 01-10-03" src="https://github.com/user-attachments/assets/ef144c86-c285-414e-a409-02568a17b41a">
  
   Penjelasan:
  - mkdir adalah perintah untuk membuat direktori.
  - -p membuat direktori bersarang jika diperlukan dan tidak akan menampilkan kesalahan jika direktori sudah ada.


3. Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari
dan copy-kan file tersebut ke sub direktori februari dan maret. 

  <img widthy="500" alt="Screenshot from 2024-09-11 01-31-44" src="https://github.com/user-attachments/assets/27c41b22-1c8a-4413-82d0-e58a415b32d1">

  <img widthy="500" alt="Screenshot from 2024-09-11 01-36-43" src="https://github.com/user-attachments/assets/1d08c05e-82b3-4aff-9287-fc70002452b7">

  Penjelasan:
  - echo -e mencetak string dengan interpretasi karakter escape (misalnya \n untuk baris baru).
  - (> mengalihkan output dari perintah echo ke file januari/dataku.txt, membuat file baru atau menimpa file yang ada.)
  - cp adalah perintah untuk menyalin file.
  - januari/dataku.txt adalah file sumber.
  - februari/ dan maret/ adalah direktori tujuan.


4. Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others 
dapat melakukan write. 

  <img widthy="500" alt="Screenshot from 2024-09-11 06-26-10" src="https://github.com/user-attachments/assets/41825eeb-098a-4e8a-bfd9-0157da558af0">

Penjelasan:

    chmod 662:
    -  6 (read + write) untuk owner.
    -  6 (read + write) untuk group.
    -  2 (write-only) untuk others.

Setelah perintah ini dijalankan:
    -  Owner (user) dapat membaca dan menulis.
    -  Group dapat membaca dan menulis.
    -  Others hanya bisa menulis (tidak bisa membaca).

  <img widthy="500" alt="Screenshot from 2024-09-11 06-27-40" src="https://github.com/user-attachments/assets/401fad34-d27c-41a8-861a-b2428e920010">

Mengecek izin akses apakah sudah berubah dengan benar
Penjelasan output:

    rw-rw--w-:
        -  Owner (peni-ilhami) memiliki izin read dan write (rw-).
        -  Group memiliki izin read dan write (rw-).
        -  Others hanya memiliki izin write (-w-), tidak bisa membaca.

5. Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat 
melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read 
dan execute. 

  <img widthy="500" alt="Screenshot from 2024-09-11 06-37-09" src="https://github.com/user-attachments/assets/ce6c7981-4b7c-4632-be89-1343a4fef729">

Penjelasan:

    chmod 754:
        -  7 (read, write, execute) untuk user (owner).
        -  5 (read, execute) untuk group.
        -  4 (read-only) untuk others.

Penjelasan output:

    rwxr-xr--:
        -  User (owner) memiliki izin read, write, dan execute (rwx).
        -  Group memiliki izin read dan execute (r-x), tetapi tidak bisa menulis.
        -  Others hanya bisa membaca dan mengeksekusi (r--), tetapi tidak bisa menulis.

    
6. Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat 
melakukan write, read dan execute.

   <img widthy="500" alt="Screenshot from 2024-09-11 06-46-59" src="https://github.com/user-attachments/assets/38a0ec5a-7060-4723-a34e-89a33e75f3fe">

Penjelasan:

    chmod 777:
        -  7 untuk user: read (r), write (w), execute (x).
        -  7 untuk group: read (r), write (w), execute (x).
        -  7 untuk others: read (r), write (w), execute (x).
Penjelasan output:

    rwxrwxrwx:
        -  User (owner) memiliki izin read, write, dan execute (rwx).
        -  Group memiliki izin read, write, dan execute (rwx).
        -  Others juga memiliki izin read, write, dan execute (rwx).
        
7. Hapuslah direktori maret. 

  <img widthy="500" alt="Screenshot from 2024-09-11 06-52-09" src="https://github.com/user-attachments/assets/af411e48-10cc-4394-98fd-d14c2ef1ab64">

  <img widthy="500" alt="Screenshot from 2024-09-11 06-52-49" src="https://github.com/user-attachments/assets/b5af087f-db49-43ce-bf1b-256f09d7d682">

rm -r: Menghapus direktori dan semua isinya secara rekursif (termasuk file dan subdirektori di dalamnya).

8. Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapat 
melakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori 
februari.

 <img widthy="500" alt="Screenshot from 2024-09-11 07-01-18" src="https://github.com/user-attachments/assets/8a67c18a-19cc-40b9-a884-bd808201d007">

Penjelasan :
-  5 untuk user (read dan execute, tanpa write).
-  4 untuk group (hanya read, tanpa execute dan write).
-  4 untuk others (hanya read, tanpa execute dan write).

    <img widthy="500" alt="Screenshot from 2024-09-11 07-05-45" src="https://github.com/user-attachments/assets/ee286d0e-b1e3-496a-9875-928a23f38253">

Penjelasan output:

    dr-xr--r--:
        -  User (owner) hanya bisa membaca dan mengeksekusi.
        -   roup hanya bisa membaca.
        -  Others hanya bisa membaca.

   <img widthy="500" alt="Screenshot from 2024-09-11 07-10-06" src="https://github.com/user-attachments/assets/0ea39b8b-44a3-411e-ac16-1539136b837f">

   Pesan ini menunjukkan bahwa perubahan izin akses sudah berhasil, dan baik user maupun group tidak dapat membuat (menulis) direktori atau file baru di dalam subdirektori
   Februari.


9. Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakan 
nilai default-nya ? 

<img widthy="500" alt="Screenshot from 2024-09-11 07-25-52" src="https://github.com/user-attachments/assets/c709dded-91f9-471f-9219-222ce4e2142f">
  
  Penjelasan027 berarti:
  
    -  User akan memiliki izin penuh (read, write, execute).
    -  Group hanya memiliki izin read dan execute (tidak bisa menulis).
    -  Others tidak memiliki izin apapun (tidak bisa membaca, menulis, atau mengeksekusi).
    -  Hasilnya akan menunjukkan umask saat ini, yang seharusnya 0027

10. Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah 
list perhatikan berapa link yang terjadi ?

 <img widthy="500" alt="Screenshot from 2024-09-11 07-39-09" src="https://github.com/user-attachments/assets/905ec8e9-3d33-48d2-8b88-54065490f803">

Penjelasan:

    -  Angka 3 sebelum nama pengguna (peni-ilhami) menunjukkan bahwa file Dataku, Dataku.ini, dan Dataku.juga memiliki tiga hard link yang menunjuk ke file yang sama.
    -  Jadi, setiap perubahan yang dilakukan pada salah satu file akan berlaku untuk semuanya karena mereka berbagi inode yang sama.
