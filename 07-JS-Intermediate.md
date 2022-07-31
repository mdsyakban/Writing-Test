## JS Intermediate

### Array
Array adalah tipe data list order yang dapat menyimpan tipe data apapun di dalamnya. Array dapat menyimpan tipe data String, Number, Boolean, dan lainnya. Array didefinisikan menggunakan square brackets. Contoh :
```
let data = ['Ini string', 20, true];
console.log(data);
```
Dalam mengakses/memanggil array dihitung dari index data ke-0. Dalam contoh di atas 'Ini string' merupakan data pertama index ke-0 dan seterusnya. Kita juga dapat mengupdate data pada suatu array. Contoh :
```
let data = ['Ini string', 20, true];

data[1] = 10;
console.log(data); // Output : ['Ini string', 10, true];
```

### Array Properties
Array memiliki 5 properti yang sering digunakan yaitu constructor, length, index, input, dan prototype. Dan pada kesempatan ini saya hanya membahas length.

- length

length akan mengembalikan nilai dari jumlah panjang data suatu array. Contoh :
```
let data = ['Ini string', 20, true];
console.log(data.length); // Output : 3
```

### Array Method
Array memiliki method atau biasa disebut built-in methods. Artinya Javascript sudah memudahkan kita dengan menyediakan function/method umum yang bisa kita gunakan. Kita tidak perlu membuat function lagi jika method yang kita butuhkan sudah tersedia. Adapun array method sebagai berikut :
- .push(), adalah method untuk menambahkan item  array pada urutan yang paling akhir.
- .pop(), adalah method yang menghapus item array index terakhir.
- .shift() adalah method untuk menghapus item Array pada index pertama.
- .unshift() adalah method untuk menambahkan item Array pada index pertama.
- .sort() adalah method untuk mengurutkan secara Ascending atau Descending Alphanumeric.

### Looping pada array
Array memiliki built in methods untuk melakukan looping yaitu :
- .forEach()
- .map()

### Multidimensional Array
Multidimensional Array bisa dianalogikan dengan array of array.
Ada array didalam array. Contoh :
```
let data =[
    ['Kaos Polos',10],
    ['Jaket', 12],
    ['Topi', 8],
];
```
### JavaScript Object
Dalam dunia Programming, object adalah sebuah tipe data pada variabel yang menyimpan properti dan fungsi (method). Properti adalah data lengkap dari sebuah object. Method adalah action dari sebuah object. Sama seperti tipe data sebelumnya. Object dapat diassign kedalam sebuah variabel. Contoh nya :
```
let person = {
    name : 'Ahmad Syakban'
    age : 22,
}
```
Sama seperti array, didalam object kita dapat menyimpan properti dengan tipe data apapun. Dalam mengakses objek, kita dapat mengakses seluruh object tersebut dan kita juga dapat mengakses properti dari object nya.
```
Mengakses seluruh object :
let person = {
    name : 'Ahmad Syakban'
    age : 22,
}

console.log(person);

Mengakses properti dari object :
let person = {
    name : 'Ahmad Syakban'
    age : 22,
}

console.log(person.name);
``` 
Kita juga bisa menggunakan bracket notation saat memanggil properti dari sebuah object.
```
let person = {
    name : 'Ahmad Syakban'
    age : 22,
}

console.log(person['name']); // Output : 'Ahmad Syakban'
```
Update Object

Kita dapat melakukan update pada variabel dengan tipe data Object. Object dapat mengupdate value dari key yang sudah tersedia dan object dapat menambahkan key dan value baru. Contoh :
```
let person = {
    name : 'Ahmad Syakban'
    age : 22,
}

// Update value dari key yang sudah tersedia :
person.age = 23;

// Menambahkan key dan value baru :
person.address = 'Sumbawa'
```
Jika menggunakan constant pada variable object. maka kita tidak bisa mengganti seluruh data object dengan object yang baru.

Delete Object Property

Kita dapat menghapus properti dari object menggunakan delete operator.
```
let person = {
    name : 'Ahmad Syakban'
    age : 23,
    address : 'Sumbawa',

    delete person.address;
}
```
Method

Jika value yang kita masukkan pada property berupa function. Maka itu disebut method.
```
const greeting = {
    welcome: function() {
        return 'Hallo selamat datang';
    },
    afterTransaction: function() {
        return 'Terima kasih sudah membeli produk kami';
    },
};

console.log(greeting.welcome()); // 'Hallo selamat datang'
```
Looping Object

Jika kita ingin menampilkan seluruh object properti. Kita bisa menggunakan looping. Jadi tidak perlu mengakses secara manual memanggil setiap propertinya. Adapun struktur nya sebagai berikut :
```
for (let key in project){
    // ...
}
```
### JavaScript Recursive
Recursive adalah function yang memanggil dirinya sendiri sampai kondisi tertentu.
Ciri-ciri rekursif :
- Fungsi rekursif selalu memiliki kondisi yang menyatakan kapan fungsi tersebut berhenti. 
- Fungsi rekursif selalu memanggil dirinya sendiri sambil mengurangi atau memecahkan data masukan setiap panggilannya. Hal ini penting diingat, karena tujuan utama dari rekursif ialah memecahkan masalah dengan mengurangi masalah tersebut menjadi masalah-masalah kecil.

### JavaScript Regex
Regex adalah susunan karakter/deretan karakter spesial yang menggambarkan pattern/pola untuk pencarian text pada sebuah string atau document.

Contoh kasus yang menggunakan Regex :
- Validasi input dari sebuah FORM
- Mencari keyword tertentu pada email atau halaman web
- Mencari IP address dalam kisaran tertentu
- Dan masih banyak lagi

### JavaScript OOP
Object Oriented Programming (OOP) adalah suatu paradigma dalam pemrograman. Kita telah mempelajari paradigma seperti procedural, conditional, hingga function.

Ada 4 hal pilar dalam OOP yaitu:
- Encapsulation

Encapsulation adalah cara untuk membatasi akses langsung ke properti atau method dari sebuah objek.
- Inheritance

Inheritance dalam OOP adalah sebuah proses dimana sebuah class mewariskan property dan methodnya ke class lain atau childnya.

- Polymorpishm

Secara bahasa, polymorphism berasal dari dua kata, yaitu poly yang berarti banyak dan morphism yang berarti bentuk. Polymorpish ini juga dikenal pada konsep OOP yang berarti kemampuan dari suatu objek untuk memiliki banyak bentuk.

Pada pilar sebelumnya yaitu inheritance, child class dapat mewarisi properti dan method dari parent class. Nah pada Polymorpishm, method yang diwariskan bisa kita ubah dengan behaviour yang berbeda menyesuaikan child class yang kita buat.
- Abstraction

Abstraction adalah sebuah teknik untuk menyembunyikan detail tertentu dari sebuah objek/method dan hanya menampilkan fungsionalitas atau fitur penting dari objek tersebut.

Analogi dari abstraction misalnya seperti ini :

Setiap hari kamu berangkat ke kantor dengan mengendarai mobil pribadimu.

Kamu sebenarnya tidak perlu tahu bagaimana mesin mobil itu bekerja sampai membuat mobilnya bisa bergerak atau bagaimana sistem pembakaran dalam mesinnya dan apa yang terjadi di dalam mesin ketika kamu menginjak pedal gas.

Yang perlu kamu tahu adalah cara menyalakan mobil dan tau cara menyetir.

### JavaScript Modules
Modules adalah reusable code yang dapat di export dari suatu file javascript dan di import ke file javascript yang lain.Reusable code disini adalah data yang dapat digunakan berulang kali. Kita dapat melakukan export pada data apapun seperti string, object, number, array, class, hingga function/method.

Sebelum menggunakan export import untuk membuat modules. Ada beberapa syarat yang harus disiapkan. Saat menjalankan modules, kita tidak bisa menggunakan url local komputer kita di browser. Harus menggunakan static server. Gunakan extension live server pada visual studio code . Lalu pada file index.html nya kita harus menambahkan script attribute type untuk modules.

Ada beberapa cara dalam melakukan export antara lain :
- Export as
- Import as
- Export default

### Web Storage
Local Storage merupakan tempat di browser yang bisa digunakan untuk menyimpan data dan tidak akan hilang walaupun browser di close. Ada 4 Metode yang dapat digunakan dalam menggunakan local storage, yaitu :
- setItem(), digunakan untuk menyimpan data ke dalam local storage.
- getItem(), digunakan untuk mengakses data yang disimpan pada localStorage.
- removeItem(), digunakan untuk menghapus data tertentu pada penyimpanan localStorage bedasarkan key.
- clear(), digunakan untuk menghapus seluruh data yang telah tersimpan di localStorage. Penggunaannya tidak perlu menuliskan key ataupun value.

Session Storage adalah menyimpan data secara sementara, data akan menghilang saat tab ditutup atau browser ditutup. Metode dalam session Storage sama halnya dengan local Storage yaitu :
- setItem()
- getItem()
- romoveItem()
- clear()

### Javascript Asynchronus
Bahasa pemrograman JavaScript termasuk ke dalam single-thread language atau synchronous yang artinya hanya dapat mengeksekusi satu perintah pada satu waktu dan harus menunggu satu perintah tersebut selesai sebelum melanjutkan perintah selanjutnya. Untuk bisa mengeksekusi urutan perintah dari kode yang kita tulis ada 2 istilah yang digunakan pada JavaScript yaitu synchronous dan asynchronous.

Synchronus, adalah saat kita mengeksekusi perintah satu persatu dan berurutan. Analoginya seperti kita sedang mengantri di kasir atau loket. Ketika ada 1 perintah masuk maka dia akan dieksekusi terlebih dahulu. Jika perintah belum selesai dan sudah ada perintah baru maka perintah kedua (yang baru) akan mengantri sampai perintah 1 selesai. 

Asynchronous, mengizinkan komputer kita untuk memproses perintah lain sambil menunggu suatu proses lain yang sedang berlangsung. Ini artinya kita bisa melakukan lebih dari 1 proses sekaligus (multi-thread). Eksekusi perintah dengan asynchronous tidak akan melakukan blocking atau menunggu perintah sebelumnya selesai. Jadi sambil menunggu kita bisa mengeksekusi perintah lain. Analoginya seperti saat kita mencuci baju di mesin cuci. Agar lebih produktif, sambil menunggu cucian selesai kita bisa melakukan pekerjaan lain misalnya menyapu dan mengepel. Artinya disini kita melakukan 3 proses sekaligus.
















