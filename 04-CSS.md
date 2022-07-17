## CSS

CSS singkatan dari Cascading Style Sheets adalah bahasa yang digunakan untuk mendesain, mempercantik halaman website. Dengan menggunakan CSS ini kita dapat merubah warna background dan font, jenis font, mengatur tata letak dan lain-lain.

### Cara menggunakan CSS :
1. Inline CSS

Inline styles adalah kita menambahkan CSS pada atribute elemen HTML.
```
<p style="color: coral; font-size: 36px;">Ini Paragraph</p>
```

2. Internal CSS

Internal CSS menggunakan element style untuk menyisipkan kode CSS. Element style diletakkan di dalam element head.
```
<head>
  <title>Internal CSS</title>
  <style>
    h1 {background-color:deepskyblue;}
  </style>
</head>
```

3. External CSS

External CSS adalah cara menyisipkan kode CSS dengan cara membuat file CSS terpisah, dan lalu menyambungkannya dengan file HTML dengan menggunakan element link. Element link tersebut diletakkan di dalam element head.
```
index.html

<!DOCTYPE html>
<html>
  <head>
    <title>External CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>

    <h1>Saya bahagia</h1>

  </body>
</html>
```
```
style.css

h1 {
    color: brown;
}
```

### CSS - Tag Name
Kita dapat menggunakan tag HTML secara langsung pada CSS. Dengan menggunakan tag element, maka ini bersifat global. Global artinya akan mempengaruhi seluruh tag element HTML yang ada pada file tersebut.
```
index.html

<body>
  <div>
    <h1>Hai this is my blog</h1>
    <p>I love learning and sharing</p>
  </div>
  <div>
    <h1>My Profile</h1>
    <ul>
      <li>Name : Ahmad Syakban</li>
      <li>Age : 22 years old</li>
      <li>Education : Sumbawa University Of Technology</li>
      <li>Major : Informatic Engineering</li>
      <li>Address : Sumbawa</Address></li>
    </ul>
  </div>
</body>
```
```
style.css
h1 {
  color : green;
}
```
Maka kedua Tag Heading h1 akan ikut berubah dengan styling yang sama.

### CSS - Class Name
Kita bisa menggunakan attribute class pada elemen HTML lalu memanggil nama class tersebut pada CSS. HTML yang memiliki class yang sama, akan mempunyai styling yang sama saat digunakan pada CSS.
```
index.html
<body>
  <div>
    <h1 class="title">Hai this is my blog</h1>
    <p>I love learning and sharing</p>
  </div>
  <div>
    <h1>My Profile</h1>
    <ul>
      <li>Name : Ahmad Syakban</li>
      <li>Age : 22 years old</li>
      <li>Education : Sumbawa University Of Technology</li>
      <li>Major : Informatic Engineering</li>
      <li>Address : Sumbawa</Address></li>
    </ul>
  </div>
</body>
```
```
style.css
.title {
  color: brown;
}
```
Walaupun kedua heading memiliki tag yang sama yaitu h1, itu tidak membuat styling yang sama untuk kedua heading h1 tersebut, karena menggunakan class. Pada pemanggilan class pada CSS diawali dengan titik (.) di ikuti nama class.

### CSS - Multiple Class
Kita dapat menggunakan lebih dari 1 class yang berbeda untuk 1 element HTML.

Contoh kasus :

Kita memiliki 2 heading. Kita ingin keduanya memiliki warna yang sama. Tapi kita ingin format heading yang satu huruf besar (uppercase) dan heading yang huruf kecil (lowercase).
```
index.html

<body>
  <div>
    <h1 class="title uppercase">Hai this is my blog</h1>
    <p>I love learning and sharing</p>
  </div>
  <div>
    <h1 class="title lowercase">My Profile</h1>
    <ul>
      <li>Name : Ahmad Syakban</li>
      <li>Age : 22 years old</li>
      <li>Education : Sumbawa University Of Technology</li>
      <li>Major : Informatic Engineering</li>
      <li>Address : Sumbawa</Address></li>
    </ul>
  </div>
```
```
style.css

.title {
  color: brown;
}

.uppercase {
  text-transform: uppercase;
}

.lowercase {
  text-transform: lowercase;
}
```
Maka heading pertama akan berwarna brown dan menjadi huruf besar, sedangkan heading kedua akan berwarna merah dan menjadi huruf kecil.

### CSS - ID Name
Berbeda dengan Class Name. ID Name bersifat unik artinya hanya ada 1 nama ID pada 1 element HTML. Biasanya digunakan jika hanya ada 1 element pada 1 page contohnya navigation, header, footer. Jadi kita bisa gunakan ID jika element tersebut unik dan hanya ada 1.
```
index.html

<body>
  <!-- ID NAVIGATION -->
  <div id="navigation">
    <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">About Me</a></li>
    <li><a href="#">My Journal</a></li>
    </ul>
  </div>
  <div>
    <h1 class="title">Hai this is my blog</h1>
    <p>I love learning and sharing</p>
  </div>
  <div>
    <h1>My Profile</h1>
    <ul>
    <li>Name : Ahmad Syakban</li>
    <li>Age : 22 years old</li>
    <li>Education : Sumbawa University of Technologi</li>
    <li>Major : Informatic Engineering</li>
    <li>Adress : Sumbawa</li>
    </ul>
  </div>
  <div>
    <h1>My Galeri</h1>
  </div>
  <img src="20200428_112033.jpg" width="400" alt="Air terjun">
</body>
```
```
style.css

.title {
  color: brown;
}

#navigation ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

#navigation li {
  display: inline;
  padding: 15px;
}

#navigation li a{
  text-decoration: none;
}
```
Gunakan tanda pagar (#) untuk memanggil element ID HTML pada CSS
Perbedaan class name dan id name :

Gunakan ID Name jika hanya ada 1 element pada file/halaman HTML contohnya navigation dan footer.

Gunakan Class Name jika akan ada beberapa element HTML yang memiliki styling/desain yang sama contohnya kita ingin Heading Blog kita memiliki styling yang sama.

### Chaining Selector
Contoh kasus :

Jika kita memiliki 2 tag element HTML pada CSS namun kita ingin ada 1 element HTML yang memiliki styling berbeda.
```
index.html

<body>
  <div>
  <!-- ELEMENT TAG HEADING <h1> -->
    <h1>Hai this is my blog</h1>
    <p>I love learning and sharing</p>
  </div>
  
  <!-- ELEMENT TAG HEADING <h1> YANG MENGGUNAKAN CHAINING SELECTOR -->
  <h1 class="titleGalery">My Galery</h1>
  <img src="image/my-photo.jpg" width="400">
</body>
```
```
style.css

/* Styling berlaku untuk semua element tag h1 */
h1 {
  color: brown;
}

/* Styling berlaku untuk semua element tag h1 yang memiliki class titleGalery */
h1.titleGalery {
  color: green;
```

### Nested Element
Konsep CSS sama dengan HTML yaitu setiap element memiliki parent dan child.
```
index.html

<body>
  <div>
    <h1>Hai this is my blog</h1>
    <p>I love learning and sharing</p>
  </div>
  
  <!-- Nested Element -->
  <div class="parentGalery">
  <h1>My Galery</h1>
  <img src="image/my-photo.jpg" width="400">
</body>
```
```
style.css

/* Child pada class parentGalery akan mengikuti styling/desain rules dari parent. Element tag heading dan image didalam class ini akan ikut berubah. */

.parentGalery {
  text-align; center;
}
```
Maka hasil nya My Galery dan juga image nya akan berada di tengah atau center.

### Multiple Selector
Sebagai seorang programmer handal, kita perlu latihan dan terbiasa membuat code yang efektif. Jangan mengerjakan code yang sama berulang kali. Pada CSS kita bisa membuat code lebih efisien dan tidak berulang-ulang.

Contoh style yang tidak menggunakan multiple selector :
```
h1 {
  color: brown;
  font-family: 'Nunito', sans-serif;
}

p {
  font-family: 'Nunito', sans-serif;
}
```
Contoh style yang menggunakan selector :
```
h1 {
  color: brown;
  font-family: 'Nunito', sans-serif;
}

h1, p {
  font-family: 'Nunito', sans-serif;
}
```
