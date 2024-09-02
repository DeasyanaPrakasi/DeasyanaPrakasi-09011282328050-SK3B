# Praktikum 1 Sistem Operasi Instalasi Sistem Operasi Linux
## Pendahuluan

Praktikum instalasi sistem operasi Linux adalah langkah penting untuk belajar bagaimana menggunakan dan mengelola sistem operasi open source ini. Linux menjadi pilihan banyak orang karena stabilitas, keamanan, dan fleksibilitasnya. Di dalam praktikum ini, kita akan mempelajari bagaimana cara menginstal Linux pada komputer atau virtual machine, mengatur konfigurasi dasar, serta mengenal perintah-perintah dasar Linux.

Sebelum memulai, kita perlu mempersiapkan beberapa hal seperti memilih distribusi Linux yang sesuai, menyiapkan media instalasi, dan memastikan komputer atau virtual machine yang kita gunakan memiliki spesifikasi yang memadai. Selain itu, kita juga akan membutuhkan koneksi internet untuk mengunduh paket-paket yang diperlukan selama instalasi.

Dalam praktikum ini, kita juga akan membahas beberapa konsep penting tentang sistem file di Linux, termasuk alasan di balik penggunaan direktori root (/) sebagai titik mount utama. Kita juga akan melihat perbedaan antara berbagai jenis sistem berkas seperti ext4, ext3, swap, NFS, FAT32, dan Btrfs. Setiap jenis sistem berkas ini memiliki fungsi dan keunggulannya sendiri, sehingga memahami kapan dan bagaimana menggunakannya sangat penting untuk pengelolaan Linux yang efektif.

## Tujuan

- Mengetahui prosedur instalasi pada sistem operasi linux

- Mampu menjalankan instalasi melalui Graphic User Interface (GUI) maupun Command Line Linux

- Mampu menganalisis proses instalasi

## Alat & Bahan

1. Laptop
   
2. Ubuntu
 
3. Virtual

## Dasar Teori

Sistem operasi Linux, yang dikembangkan oleh Linus Torvalds pada tahun 1991, adalah sistem operasi open source berbasis Unix yang bisa dijalankan di berbagai jenis perangkat keras. Salah satu keunggulan Linux adalah fleksibilitasnya, yang memungkinkan pengguna untuk menginstal dan mengonfigurasi sistem sesuai kebutuhan mereka. Linux dikenal karena stabilitas, keamanan, dan kemampuannya untuk disesuaikan, dengan struktur sistem file yang diatur secara hierarkis dan menggunakan direktori root (/) sebagai pusat dari semua direktori dan file lainnya. Memahami struktur ini sangat penting untuk memastikan sistem Linux berfungsi dengan baik dan efisien.

Linux juga menggunakan berbagai jenis sistem berkas, masing-masing dengan fungsi dan keunggulannya sendiri. Memilih sistem berkas yang tepat sangat penting karena akan memengaruhi kinerja dan stabilitas sistem. Sistem berkas ini menentukan bagaimana data disimpan, diakses, dan dikelola oleh sistem operasi, sehingga pemilihan yang tepat adalah langkah kunci dalam pengelolaan Linux yang efektif.

## Pembahasan
### Instalasansi Ubuntu

Untuk menginstal Ubuntu di VirtualBox, ikuti langkah-langkah berikut:

1. **Persiapan:**
   -  Kunjungi situs web Ubuntu dan download file ISO dari versi Ubuntu yang terbaru.
   -  Download dan instal Oracle VM VirtualBox dari situs web resminya.

2. **Buat Mesin Virtual di VirtualBox:**
   -  Jalankan aplikasi VirtualBox.
   -  Klik tombol “New” untuk membuat mesin virtual baru.
    
        ![Screenshot (635)](https://github.com/user-attachments/assets/3a80a0dc-f01f-4d83-8344-e0f5ab8b8ac8)

   - Masukkan nama untuk mesin virtual (misalnya, “Ubuntu”), pilih tipe “Linux” dan versi “Ubuntu (64-bit)”.
   
        ![Screenshot (629)](https://github.com/user-attachments/assets/c3fe06d8-5c8d-4803-a234-c176f95a587f)

   -  Pilih jumlah RAM yang akan dialokasikan untuk mesin virtual. 
   -  Pilih opsi “Create a virtual hard disk now” .
   -  Pilih “VDI (VirtualBox Disk Image)” dan klik “Next”.
     
        ![Screenshot (631)](https://github.com/user-attachments/assets/d3cb05ed-632d-4b51-b348-88619093ce4c)
        ![Screenshot (630)](https://github.com/user-attachments/assets/63212e35-2af6-42f7-b972-2bd4c8559d77)


3. **Konfigurasi Mesin Virtual:**
   -  Pilih mesin virtual yang baru dibuat dari daftar dan klik “Settings”.
   -  Atur Media Instalasi
     
        ![Screenshot (633)](https://github.com/user-attachments/assets/bbea2dd7-5ec4-46b9-bf9f-a7226c291d31)

     - Klik “Storage” di panel kiri.
     - Klik ikon disk kosong di bawah “Controller: IDE”, lalu klik ikon disk di sebelah kanan dan pilih “Choose a disk file”. Pilih file ISO Ubuntu yang telah diunduh.
       
          ![Screenshot (634)](https://github.com/user-attachments/assets/517406da-75fe-427d-8738-d5f4e46490a0)


4. **Instal Ubuntu:**
   -  Klik “Start” untuk menjalankan mesin virtual.
   -  Ketika mesin virtual boot dari ISO Ubuntu, pilih “Try and Install Ubuntu” pada layar instalasi Ubuntu.
     
        ![IMG-20240902-WA0002](https://github.com/user-attachments/assets/d77a4eb7-ed8f-42e3-966e-7624cb461331)

   - Pilih bahasa dan lokasi sesuai preferensi.
       
        ![IMG-20240902-WA0004](https://github.com/user-attachments/assets/dbf07c6e-9d07-4c0a-ac15-40bd06e1f48d)
       

   - Pilih opsi untuk terhubung ke internet jika diperlukan.
       
       ![IMG-20240902-WA0026](https://github.com/user-attachments/assets/07a034fb-b934-4b54-b52b-d23d8c92c3b1)

   - Pilih opsi “Erase disk and install Ubuntu” untuk menginstal Ubuntu di hard disk virtual.
       
       ![IMG-20240902-WA0007](https://github.com/user-attachments/assets/0477fbeb-056c-4ede-95cd-9a7d6cb25c7c)

   - Ubuntu akan secara otomatis mengatur partisi pada hard disk virtual. Pilih “Install Now” untuk melanjutkan.
  
        ![IMG-20240902-WA0025](https://github.com/user-attachments/assets/573835b2-cc6c-4c43-a42a-a8b5b7ec7415)

   - Masukkan informasi seperti nama, nama pengguna, dan kata sandi.
  
       ![IMG-20240902-WA0031](https://github.com/user-attachments/assets/734dea31-6343-4776-8188-47f1bdf18ce4)

   - Tunggu hingga proses instalasi selesai. Ini akan memakan waktu beberapa menit.

       ![IMG-20240902-WA0029](https://github.com/user-attachments/assets/9fc687b2-30c5-4b9a-af28-db97295809c8)
     
5. **Selesai dan Reboot:**
   - Setelah instalasi selesai, Anda akan diminta untuk me-restart mesin virtual. Klik “Restart Now”.

6. **Gunakan Ubuntu:**
   - **Masuk ke Ubuntu:**  masuk menggunakan akun yang telah dibuat selama instalasi.
   



