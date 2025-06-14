# TASK-SETUP-ANACONDA-UV
-----

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


-----

# Bagian 2:Membuat UV

1. Buat Environment Baru

	**Apa**
	Membuat environment terisolasi untuk proyek UV.

	**Kenapa**
	Agar dependensi proyek tidak bentrok dengan proyek lain.

	Langkah-langkah:
	1.	Pastikan lingkungan Conda tidak aktif (jalankan conda deactivate jika perlu).
	2.	Ketik: pip install uv
	3.	Output seperti Successfully installed uv-0.7.12 menunjukkan keberhasilan.
	4.	Catatan tentang folder ghost_intellixuv: Folder ghost_intellixuv akan dibuat di langkah berikutnya  menggunakan uv init. Perintah ini otomatis membuat folder 		jika belum ada, karena UV dirancang untuk menginisialisasi direktori proyek baru secara langsung. Anda tidak perlu membuat folder ini secara manual sebelum 			menjalankan uv init. Untuk memverifikasi folder setelah inisialisasi, ketik dir di CMD untuk melihat daftar direktori.


 ![image](https://github.com/David-rohmannudin/TASK-SETUP-ANACONDA-UV/blob/main/Task-Anaconda/CMD%20PIP%20UV.png)



	Do's:
	- Beri nama environment yang deskriptif
	- Gunakan versi Python yang kompatibel

	Don'ts:
	- Jangan gunakan environment base untuk proyek
	- Jangan membuat terlalu banyak environment yang tidak perlu


# 2. Menginisialisasi Proyek UV

   **Apa?**
Menginisialisasi Proyek UV adalah proses mempersiapkan struktur direktori dan file konfigurasi dasar untuk proyek yang akan menggunakan UV environment. Ini termasuk membuat file requirements, struktur folder, dan konfigurasi dasar proyek.

**Kenapa?**
Inisialisasi proyek yang benar membantu menjaga konsistensi struktur proyek, memudahkan kolaborasi tim, dan memastikan semua dependensi terkelola dengan baik. Ini juga mempermudah deployment dan reproduksi environment di mesin lain.

Langkah-langkah:
1. Pastikan environment UV sudah aktif
2. Ketik: uv init ghost_intellixuv
           Cd ghost intellixuv
3. Output menunjukkan proyek diinisialisasi di C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv.

![image](https://github.com/David-rohmannudin/TASK-SETUP-ANACONDA-UV/blob/main/Task-Anaconda/cmd%20ghost.png)


	Do's:
	- Gunakan struktur folder yang konsisten
	- Dokumentasikan semua dependensi di requirements.txt
	- Buat README.md yang jelas
	- Gunakan virtual environment untuk setiap proyek	

	Don'ts:
	- Jangan mencampur file proyek dengan file personal
	- Jangan lupa menambahkan environment ke .gitignore
	- Jangan menyimpan data sensitif di direktori proyek
	- Jangan mengubah struktur folder setelah proyek berjalan


# 3. Instal Paket yang Dibutuhkan 

**Apa?**
Memasang library yang diperlukan untuk proyek UV.

**Kenapa?** 
Untuk mendapatkan fungsi-fungsi yang dibutuhkan dalam pengembangan.

	Langkah-langkah:
	Ketik: uv add pandas

![image](https://github.com/David-rohmannudin/TASK-SETUP-ANACONDA-UV/blob/main/Task-Anaconda/install%20paket%20.png)


Do's:
- Install hanya paket yang diperlukan
- Periksa versi paket yang kompatibel

Don'ts:
- Jangan install paket di environment base
- Jangan install paket tanpa memeriksa dependensinya
- Jangan campur UV dan pip.

# 4. Nonaktifkan Lingkungan UV

**Apa?**
Nonaktifkan environment uv_env apabila sudah selesai menggunakan.

**Kenapa?**
Agar shell kembali ke environment base atau default.

Langkah-langkah:
1.	Ketik: .venv\Scripts\deactivate
2.	Prompt kembali ke C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv>.

![image](https://github.com/David-rohmannudin/TASK-SETUP-ANACONDA-UV/blob/main/Task-Anaconda/nonafktifkan%20uv.png)




# 6. Perbandingan Conda VS UV

**Apa?**
Membandingkan manajemen environment Conda dengan framework UV (asumsi UV adalah sistem manajemen environment atau framework spesifik).

**Kenapa?**
Agar memudahkan pemilihan tools sesuai kebutuhan.

	Detail:
	- Conda: manajemen environment dan paket secara umum, lintas proyek.
	- UV: environment/framework yang lebih spesifik untuk proyek tertentu, mungkin terkait AI.


	Do's:
	- Gunakan Conda untuk manajemen environment yang luas.
	- Gunakan UV jika spesifik proyek atau framework tersebut.

	Don'ts:
	- Jangan mencampur konfigurasi environment yang berbeda tanpa sinkronisasi.






	


 

