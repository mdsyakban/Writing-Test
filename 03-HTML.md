## HTML
HTML adalah singkatan dari Hypertext Markup Languange, html digunakan untuk menampilkan konten pada browser. Contoh konten yang dapat ditampilkan seperti Text, Image, Video, Link, dan masih banyak lagi.

HTML bersifat statis, ia hanya bertugas untuk menampilkan konten yang diminta oleh developer. Html ini sendiri bukanlah suatu bahasa pemrograman, yang artinya HTML tidak bisa dinamis dalam mengolah suatu data.

Dalam membuat HTML, ada 2 tools utama yang harus dipersiapkan terlebih dahulu :

1. Browser
2. Code Editor

### Dasar - Dasar HTML

Kita bisa menuliskan HTML tanpa structure dan kita tetap akan bisa menjalankannya akan tetapi untuk menjalankannya dengan baik maka kita perlu HTML structure. Contoh HTML tanpa structure :
```
Saya sedang belajar HTML
```
### HTML Structure

HTML harus memiliki struktur dasar yang terdiri dari 4 bagian utama yaitu tag DOCTYPE, tag html, tag head, tag body. 4 Bagian tersebut adalah syarat minimal yang menjadi standar pada struktur global dokumen HTML.
```
<!DOCTYPE html>
  <html>
  <head>
    <title>Judul Halaman Web</title>
  </head>
<body>
   <p>Konten halaman web.</p>
</body>
</html>
```

### HTML Anatomy
```
<tagpembuka>Isi konten</tagpenutup>
```

### HTML Element
Pada section HTML Anatomy sebelumnya, HTML Element dapat didefinisikan dengan tagpembuka, konten, dan tagpenutup. Berikut contoh HTML Element.
```
<body>
  <div>
   <!-- Element heading -->
   <h1>Konten</h1>

   <!-- Element paragraph -->
   <p>Konten</p>

   <!-- Element link -->
   <a href="https://google.com">Menuju google.com</a>
  </div>
</body>
```

### HTML Comment
HTML Comment digunakan untuk memberikan penjelasan maksud dari line code yang kita kerjakan. Comment ini selalu ada dalam bahasa pemrograman apapun. Comment tidak akan di eksekusi oleh sistem, comment hanya untuk dibaca oleh sesama programmer.
```
<body>
 <div>
  <!-- Ini adalah sintax comment HTML -->
 </div>
</body>
```

### Cara membaca dokumentasi
Untuk dapat melihat seluruh element yang ada di HTML, kita bisa cek dokumentasi yang disediakan oleh HTML seperti.
```
Resource by Mozilla
Documentation by W3schools
```