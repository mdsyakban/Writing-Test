## Responsive Web Design
### Apa itu RWD ?: 
- RWD yaitu singkatan dari Responsive Web Design. 
- RWD bertujuan membuat design website kita dapat diakses dalam device appaun. seperti Device yang umumnya digunakan adalah laptop/PC, Smartphone, dan Tablet.
- Seorang developer website wajib menggunakan tools bawaan dari setiap browser yang memudahkan proses development website , pada browser chorme biasa disebut dengan Chrome Dev Tools.

### Cara Mengakses Chrome Dev Tools
![](Gmbr1.png)
`                       
- *Jika tidak menggunakan responsive pada website kita maka panjang image menjadi overflow karena mengikuti width real bawaan dari file image*. 


### Menggunakan Max-width element.  
### Add styling max-width.
 ![](Gmbr2.png)    
- dengan menggunakan max-width maka tidak ada overflow width pada image. dan tampilan mobile device menyesuaikan dengan baik.


### Media query untuk responsive web design umumnya hanya menggunakan 2 jenis media query.
1. MIN-WIDTH
- @media screen and (min-width: your pixel) {
    /* didalam element html dan css
}
2. MAX-WIDTH
- @media screen and (max-width: your pixel) {
    /* didalam element html dan css
}
### Ada dua cara/pattern dalam menggunakan media query
1. membuat file css berbeda untuk masing" device.
- ada dua file css yaitu:
- main.css 
``` 
body {
    background-color: white;
}
```
- main.mobile.css.
``` 
body {
    background-color: aquamarine;
}
```
2. kita menggabungkan 1 file css untuk setting styling berbagai device.

![](Gmbr3.png)


### Breakpoint
- Breakpoint yaitu perubahan yang terjadi pada tampilan saat berganti device atau ukuran width.
- Ada tiga tampilan yg berbeda untuk 3jenis device. 
### Complex Breakpoint Media Query
- Jika kta ingin tampilan yg diterapkan pada range ukuran device tertentu, kita bisa membuat menjadi range media query.
- Menggunakan range media query min dan max.
![](Gmbr4.png)
Dari gambar diatas menjelaskan jika kita menggunakan media query dengan ukuran min-widht 500 dan max-width 700 maka tampilan website akan lebih besar dibandingkan dengan ukuran min-width 500 jauh lebih kecil.

## Bootstrap Grid
- HTML
```
<div class="container text-center">
  <div class="row">
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
  </div>
</div>
```

Hasilnya:

![](Gmbr5.png)

*Contoh di atas membuat tiga kolom dengan lebar yang sama di semua perangkat dan area pandang menggunakan kelas kisi yang telah ditentukan sebelumnya. Kolom tersebut dipusatkan di halaman dengan induknya .container*.

**Sistem grid Bootstrap dapat beradaptasi di keenam breakpoint default, dan setiap breakpoint yang Anda sesuaikan. Enam tingkatan grid default adalah sebagai berikut:**

1. Ekstra kecil (xs)
2. Kecil (sm)
3. Sedang (md)
4. Besar (lg)
5. Ekstra besar (xl)
6. Ekstra ekstra besar (xxl)

