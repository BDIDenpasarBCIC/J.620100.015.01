# Perintah Dasar Git

## Definisi Git

Git adalah distributed software version control yang paling banyak digunakan oleh developer dan programmer. Dengan Git mengelola source codes dalam sebuah project atau program menjadi mudah baik jika bekerja secara individu atau dalam sebuah team. 

## Mengapa kita memerlukan Git

Beberapa kegunaan Git bagi Developer atau Programmer:

* Melakukan tracking history sebuah files
* Melakukan revert process terhadap source codes
* Membuat beberapa versi berbeda dalam satu program atau project yang sama

## Fitur Git

* Distributed, artinya kita tidak perlu terhubung ke satu server tertentu untuk bisa menggunakan Git
* Offline, artinya kita tidak perlu selalu terhubung secara online untuk bisa menggunakan Git. Kita hanya perlu online jika ingin melakukan proses ``pull`` dan ``push`` dari remote repository

## Inisiasi Project (Repository)

Program atau project di Git disebut Repository. Untuk menjalankan perintah-perintah di Git, kita bisa jalankan dari console/terminal atau command line. Sebagai alternatif, terdapat beberapa software GUI untuk memudahkan kita menjalankan perintah Git.

Buka command line/console/terminal, buatlah sebuah folder baru untuk meletakkan file-file source code

```

```

Ketikan perintah 

``git init`` 

untuk inisiasi project.

Git akan membuat sebuat folder bernama ``.git`` untuk menyimpan referensi dan konfigurasi project. Pada tahap ini folder kita sudah menjadi ``repository`` git yang siap digunakan.

## Menambahkan files ke dalam Staging

Sebelum perubahan di file tercatat di Git, kita harus memasukan file tersebut ke dalam tahap staging. dengan mengetik 

``git add namafile`` 

dimana namafile adalah nama file yang akan kita staging. Jika kita ingin memasukan semua file di folder tersebut ketik

``git add .``

untuk memasukan beberapa file saja

``git add file1 file2 file3``

Setelah file yang ingin kita tracking sudah masuk ke dalam tahap staging, proses selanjutnya adalah bekerja seperti biasa menggunakan IDE atau text editor. Untuk setiap perubahan di file, kita harus menjalankan perintah ``git add`` agar perubahan yang sudah dilakukan masuk ke dalam tahap staging

## Proses Commit

Tahap selanjutnya setelah menambahkan file ke tahap staging, adalah merekam perubahan tersebut agar bisa disimpan history/log dari perubahan itu. Ketik

``git commit -m 'catatan perubahan file'``

Pada tahap ini, seluruh perubahan file telah terekam dan proses kembali diulang, mulai dari ``git init`` dilanjutkan dengan ``git commit -m 'pesan perubahan'``

Penting di ingat untuk membuat pesan perubahan atau *log message* singkat dan jelas. Pesan perubahan yang bagus adalah tidak terlalu panjang tapi singkat agar nanti ketika kita mereview perubahan-perubahan sebelumnya, kita bisa mengingat perubahan apa yang dilakukan di file tersebut.

Contoh *log message* yang bagus:

``git commit -m 'Memperbaiki tampilan di mobile sehingga menu tidak overlapping'``

Contoh *log message* yang **tidak bagus**:

``git commit -m 'ada perubahan'``

## Melihat history

Untuk melihat perubahan-perubahan apa saja di dalam sebuah repository ketik

``git log``

## Konsep Branch

Branch dalam analogi umum adalah cabang atau kelas, dalam lingkup programming atau *Software Development Lifecycle* disingkat SDLC, konsep branch artinya kita bisa memiliki beberapa versi berbeda dari sebuah program namun tetap berasal dari satu source code yang sama. Dengan fitur versioning, cukup dengan satu source code yang sama kita bisa memiliki versi ``develop`` ``beta`` ``hotfix`` ``production`` dan seterusnya.

Keuntungan dari beberapa branch yang berbeda:

* Kita bisa menambahkan fitur baru di branch berbeda tanpa harus merubah source code yang sudah live/production, dengan demikian kemungkinan error di production bisa kita hindari
* Melakukan perbaikan di branch tertentu tanpa harus merubah branch lain yang mungkin sedang dikerjakan oleh rekan developer lain. Di Git, saat pertama kali kita membuat repository hanya terdapat satu branch yang bernama ``master``

Untuk melihat branch yang ada ketik

``git branch``

Untuk membuat branch baru dan masuk ke dalam branch tersebut, ketik:

``git checkout -b namabranchbaru``

## Hosting Repository di Github



## Push dan Pull dari Github



## Solusi Conflict