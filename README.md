# PENI-ILHAMI_0901118232810.Tugas3-Sistem-Operasi
  <div align="center">

## Tugas Praktikum 3 Sistem File (File System)
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

### Langkah-Langkah

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
  - > mengalihkan output dari perintah echo ke file januari/dataku.txt, membuat file baru atau menimpa file yang ada.
  - cp adalah perintah untuk menyalin file.
  - januari/dataku.txt adalah file sumber.
  - februari/ dan maret/ adalah direktori tujuan.


4. Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others 
dapat melakukan write. 
5. Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat 
melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read 
dan execute. 
6. Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat 
melakukan write, read dan execute. 
7. Hapuslah direktori maret. 
8. Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapat 
melakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori 
februari.
9. Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakan 
nilai default-nya ? 
10. Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah 
list perhatikan berapa link yang terjadi ?

