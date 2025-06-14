# TASK-SETUP-ANACONDA-UV
**-----**

#### **Nama** : David Rohmannudin

#### **No Absen** : 10.036.DB2025

-----

## Mari sama-sama belajar setup Anaconda UV
Halo guys 🙌
yuk kita sama-sama belajar cara setup anaconda uv, 
ikuti setiap langkahnya yaaa! 

-----


## Mengenal dan Instalasi Anaconda 🐍


## Apa itu Anaconda dan Conda ?

**Anaconda** adalah distribusi open-source untuk bahasa pemrograman Python dan R, yang dirancang untuk komputasi ilmiah, analisis data, dan pembelajaran mesin. Anaconda menyederhanakan manajemen paket dan lingkungan, serta mendukung lebih dari 1.500 paket data science yang siap pakai.

**Conda** adalah manajer paket dan lingkungan yang disertakan dalam Anaconda. Conda memungkinkan pengguna untuk mengelola paket dan lingkungan secara efisien, menghindari konflik dependensi, dan memastikan konsistensi proyek.


## Apa itu UV ?
**UV** adalah alat manajemen lingkungan Python yang memungkinkan pembuatan, pengelolaan, dan penghapusan lingkungan virtual dengan mudah. Berbeda dengan pip dan virtualenv, UV mengintegrasikan pembuatan lingkungan dan instalasi paket dalam satu perintah, serta menyediakan pengelolaan versi Python secara otomatis.


## Langkah-langkah Setup Anaconda dan UV

## 🐍 Bagian 1. INSTALASI ANACONDA
## 1. Download Installer Anaconda
langkah pertama yang kita lakukan yaitu **⬇️Download Anaconda** disitus resmi

- ini merupakan link resminya guys 👉 : (https://www.anaconda.com/products/distribution ) 
- pilih versi sesuai OS Anda (Windows/macOS/Linux)
- Klik tombol Download

![image](https://github.com/David-rohmannudin/TASK-SETUP-ANACONDA-UV/blob/main/Task-Anaconda/download%20miniconda%20(39).png)


   Do:
   	- Download dari situs resmi Anaconda
	
   Don't:
   	- Jangan download dari sumber tidak resmi


    
## 2. Jalankan Installer Anaconda 📌
Langkah-langkah pemasangan Anaconda ke sistem :
- Buka file installer yang sudah didownload
- Ikuti wizard instalasi
- Pilih opsi "Add Anaconda to PATH" (opsional)

 
![image](https://github.com/David-rohmannudin/TASK-SETUP-ANACONDA-UV/blob/main/Task-Anaconda/conda%20location%2C.png)


Do's ✅: 	

- Jika tidak yakin, gunakan pengaturan default 
- Jika ingin bisa diakses dari terminal manapun centang opsi PATH 

Don'ts ❌:
- Jangan ubah direktori instalasi ke folder sistem 
- Jangan batalkan proses instalasi di tengah jalan


## 3. Verivikasi Anaconda ♾️
Lakukan verivikasi anaconda untuk memastikan bahwa anaconda memang sudah benar-benar terpasang dan dapat dipanggil dari terminal,
memverivikasi anaconda bertujuan Agar kita tidak menemui masalah di langkah selanjutnya saat menggunakan conda atau Python dari Anaconda.


	Langkah-langkah:
	1. Buka terminal atau command prompt.
	2. Ketik perintah:
	   conda --version
	3. Jika muncul versi conda, instalasi sudah sukses.
 

   ![image](https://github.com/David-rohmannudin/TASK-SETUP-ANACONDA-UV/blob/main/Task-Anaconda/conda%20version.png)


 	Do's:
		- Gunakan terminal baru setelah instalasi untuk memastikan variabel PATH terbaru terbaca   - Pastikan perintah dijalankan tanpa error.
	Don'ts:
		- Jangan abaikan error atau tidak muncul versi, cek pemasangan kembali.


### 4. Konfigurasi Variabel Lingkungan PATH Conda dan Anaconda

	Langkah-langkah:
	1. Pada Windows, tambahkan direktori Anaconda dan Scripts ke PATH Environment Variable.
	2. Pada macOS/Linux, biasanya otomatis terpasang. Jika tidak, edit .bashrc atau .zshrc untuk menambah PATH
	3. Tekan Windows + R, ketik sysdm.cpl, tekan Enter.
	4. Pergi ke tab "Advanced", klik "Environment Variables".
	5. Pilih "Path" di "System variables", klik "Edit".
	6. Tambahkan (ganti NAMA_ANDA):
	7. Klik Ok


![image](https://github.com/David-rohmannudin/TASK-SETUP-ANACONDA-UV/blob/main/Task-Anaconda/edit%20environment%20.png)
 

Do's:
- Pastikan sudah menutup dan membuka terminal baru setelah konfigurasi.
- Restart komputer jika perlu.

Don'ts:
- Jangan menghapus PATH penting lainnya.
- Hati-hati saat edit variabel lingkungan.



## 5. Membuat Lingkungan Conda Baru
Membuat environment Conda baru adalah membuat ruang kerja terpisah untuk project yang berbeda, yang bertujuan Untuk menghindari bentrok antar versi Python atau paket yang digunakan oleh berbagai proyek.

      jalan kan perintah Berikut pada cmd : 👉  conda create -n nama_env python=3.9


 ![Image](https://github.com/David-rohmannudin/TASK-SETUP-ANACONDA-UV/blob/main/Task-Anaconda/conda%20baru%20.png)

 
 
       Do's:
       - Gunakan nama environment yang deskriptif dan mudah diingat.
       - Jangan buat environment tanpa kebutuhan.

       Don'ts:
       - Jangan install semua paket di environment base.


**-----**

# Bagian 2:Membuat UV





	


 

