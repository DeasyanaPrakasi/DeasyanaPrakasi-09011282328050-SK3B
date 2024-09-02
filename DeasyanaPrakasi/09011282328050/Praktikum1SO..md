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
   -  Klik tombol “Baru” untuk membuat mesin virtual baru.
    
        ![Screenshot (635)](https://github.com/user-attachments/assets/3a80a0dc-f01f-4d83-8344-e0f5ab8b8ac8)

   - Masukkan nama untuk mesin virtual (misalnya, “Ubuntu”), pilih tipe “Linux” dan versi “Ubuntu (64-bit)”.
   
        ![Screenshot (629)](https://github.com/user-attachments/assets/c3fe06d8-5c8d-4803-a234-c176f95a587f)

   -  Pilih jumlah RAM yang akan dialokasikan untuk mesin virtual. 
   -  Pilih opsi “Buat Sebuah Virtual Sekarang” .
   -  Pilih “VDI (VirtualBox Disk Image)” dan klik “Lanjut”.
     
        ![Screenshot (631)](https://github.com/user-attachments/assets/d3cb05ed-632d-4b51-b348-88619093ce4c)
        ![Screenshot (630)](https://github.com/user-attachments/assets/63212e35-2af6-42f7-b972-2bd4c8559d77)


3. **Konfigurasi Mesin Virtual:**
   -  Pilih mesin virtual yang baru dibuat dari daftar dan klik “Pengaturan”.
   -  Atur Media Instalasi
     
        ![Screenshot (633)](https://github.com/user-attachments/assets/bbea2dd7-5ec4-46b9-bf9f-a7226c291d31)

     - Klik “Storage” di panel kiri.
     - Klik ikon disk kosong di bawah “Pengendali: IDE”, lalu klik ikon disk di sebelah kanan dan pilih “Choose a disk file”. Pilih file ISO Ubuntu yang telah diunduh.
       
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

## Pentingnya saat instalasi memilih “/” pada opsi Mount Point 
   
Memilih “/” sebagai opsi Mount Point saat menginstal Linux sangat penting karena ini adalah tempat utama di mana seluruh sistem operasi akan disimpan. Partisi dengan mount point "/" adalah tempat di mana semua file sistem, aplikasi, dan struktur direktori seperti `/home` dan `/etc` akan berada. Ini memastikan bahwa semua bagian sistem operasi tersimpan dengan rapi dan sistem berjalan dengan baik. Tanpa partisi ini, sistem operasi tidak akan memiliki tempat untuk disimpan dan tidak bisa berfungsi dengan benar.

Selain itu, memilih "/" juga mempengaruhi bagaimana ruang disk dikelola dan bagaimana sistem dipelihara. Jika Anda hanya memiliki satu partisi dengan mount point "/", semua data sistem operasi akan berada di situ, membuat pencadangan dan pemulihan lebih mudah. Dalam pengaturan yang lebih kompleks, Anda mungkin memilih untuk memisahkan data pengguna dari sistem operasi, misalnya dengan membuat partisi terpisah untuk `/home`. Ini bisa membantu dalam mengelola ruang disk dan menjaga data tetap aman.

## penjelasan Mengenai ext4, ext3, swap, ntfs, fat32,btrfs 


- ext4 (Fourth Extended Filesystem):

ext4 adalah sistem file utama di Linux yang menawarkan kinerja dan keahandalan yang lebih baik dibandingkan dengan pendahulunya, ext3. Dengan dukungan untuk volume hingga 1 Exabyte dan file hingga 16 Terabyte, ext4 juga memperkenalkan fitur seperti delayed allocation dan extents untuk meningkatkan efisiensi penyimpanan dan kecepatan akses data.

- ext3 (Third Extended Filesystem):

ext3 adalah sistem file yang menambahkan dukungan untuk sistem jurnal pada ext2, meningkatkan keandalan dengan mencatat perubahan sebelum diterapkan. Ini memungkinkan pemulihan data setelah crash dan mendukung volume hingga 16 Terabyte serta file hingga 2 Terabyte. ext3 menyediakan kompatibilitas yang baik dengan ext2, mempermudah upgrade dari versi sebelumnya.

- swap:

Swap adalah ruang di hard drive yang digunakan sebagai memori virtual oleh sistem operasi ketika RAM fisik penuh. Ini memungkinkan sistem untuk menyimpan data yang tidak aktif dari RAM ke disk, membantu meningkatkan kinerja dengan menyediakan ruang tambahan untuk proses yang sedang berjalan. Ukuran swap yang disarankan biasanya berkisar antara 1 hingga 2 kali ukuran RAM sistem.

- NTFS (New Technology File System):
  
NTFS adalah sistem file yang dikembangkan oleh Microsoft untuk sistem operasi Windows, menawarkan fitur canggih seperti enkripsi, kompresi, dan kontrol akses berbasis ACL. NTFS mendukung file dan volume yang sangat besar, menjadikannya pilihan utama untuk Windows versi terbaru dengan kinerja dan stabilitas yang baik.

- FAT32 (File Allocation Table 32):
  
FAT32 adalah sistem file yang lebih sederhana dan lebih lama dibandingkan NTFS dan exFAT. Ini sering digunakan pada perangkat penyimpanan eksternal seperti flash drive dan kartu SD karena kompatibilitas luas dengan berbagai sistem operasi. Namun, FAT32 memiliki batasan dalam hal ukuran file (hingga 4 GB) dan volume (hingga 2 Terabyte).

- btrfs (B-tree File System):
  
btrfs adalah sistem file modern untuk Linux yang dirancang untuk memberikan fitur-fitur canggih dan manajemen data yang fleksibel. Ini menawarkan dukungan untuk snapshot dan kloning, memungkinkan pencadangan dan pemulihan data yang lebih mudah. btrfs juga menyediakan integritas data melalui checksumming dan kemampuan untuk mengelola volume secara dinamis dengan fitur seperti RAID dan kompresi.


