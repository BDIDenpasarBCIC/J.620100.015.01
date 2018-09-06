# Konsep Software Version Control (SVC)

*Software version control* sering disebut juga dengan *revision control* adalah software yang digunakan oleh programmer atau developer untuk mengelola files dalam sebuah project/program agar setiap perubahan source code, penambahan atau pengurangan files/folder bisa tercatat dalam urutan revisi dan log sehingga proses tracking atau history dari sebuah file dapat dilacak.

## Pentingnya SVC

Dengan adanya pencatatan revisi/log serta history files/folder maka setiap perubahan yang terjadi didalam source code dapat diketahui mulai dari awal pembuatan source code hingga saat ini. Hal ini sangat berguna jika bekerja dalam sebuah team dimana satu file bisa dikerjakan secara bersama-sama tanpa terjadi konflik. 

Beberapa manfaat penggunaan SVC :

* Melihat history files, siapa yang melakukan perubahan dan apa yang dirubah
* Proses revert files, merubah source code ke revisi sebelumnya
* Membuat environment yang berbeda agar tidak terjadi conflict

## Jenis-jenis SVC yang Populer

### Git

Git adalah software SVC berlisensi open-source yang saat ini paling banyak digunakan karena memiliki keunggulan dibanding SVC yang lain yaitu :

* Distributed, bisa digunakan tanpa harus terkoneksi dengan server central
* Offline, bisa digunakan tanpa harus terkoneksi online
* Simple to start, bisa langsung digunakan bagi pemula dengan hanya beberapa perintah dasar

### Subversion (SVN)

SVN adalah software SVC berlisensi open-source merupakan fork dari CVS dengan penambahan fitur branch

### Concurrent Versions System (CVS)

CVS adalah software SVC berlisensi open-source yang paling awal dibuat menggunakan konsel client-server sehingga pengguna harus terhubung online

