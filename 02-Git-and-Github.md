## Git and Github

Git adalah suatu aplikasi yang dapat melacak suatu perubahan yang terjadi pada suatu folder atau file. Git biasanya digunakan oleh para programmer sebagai wadah untuk menyimpan file pemrograman, karena git ini lebih efektif. File-file yang disimpan menggunakan git akan terlacak seluruh perubahannya, termasuk siapa yang mengubah atau mengedit nya.

Github adalah sebuah situs web dan layanan berbasis cloud bagi para programmer untuk menyimpan dan mengelola kode, serta mendokumentasikan dan mengontrol perubahannya.

## Penggunaan

- Cek apakah instalasi berhasil :
```
git -- version
```
- Membuka git dapat dilakukan dengan cara :
```
Dapat menggunakan command prompt (cmd)
Dapat menggunakan powershell
Dapat menggunakan git bash
```
- Configurasi git
```
git config --global user.name "Ahmad Syakban"
git config --global user.email ahmadsyakban240@gmail.com
```
- Melihat hasil konfigurasi :
```
git config --list
```
- Inisialisasi repository :
```
git init
```
Note : Lakukan di dalam folder proyek

- Cek status :
```
git status
```
- Mendaftarkan file :
```
git add namafile.eksentsi
```
Ini berlaku apabila hanya ada 1 file yang akan di daftrakan. Tapi apabila jumlah file yang akan didaftarkan jumlah nya banyak maka kita bisa menggunakan perintah seperti ini
```
git add.
```
- Menyimpan perubahan ke dalam version control :
```
git commit -m "Pesan Commit" 
```
Mengirimkan ke version control :
```
git push -u origin master
```







