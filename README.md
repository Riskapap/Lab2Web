# Praktikum 2 - Pemograman Web 
```
Riska Puspa Anggraeni Putri 
TI.19.A2
311910440
```
## Langkah 1
### Membuat dokumen HTML dengan nama file lab2_css_dasar.html. Setelah itu buat struktur dasar HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>CSS Dasar</title>
</head>
<body>
 <header>
 <h1>CSS Internal dan <i>Inline CSS</i></h1>
 </header>
 <nav>
 <a href="lab2_css_dasar.html">CSS Dasar</a>
 <a href="lab2_css_eksternal.html">CSS Eksternal</a>
 <a href="lab1_tag_dasar.html">HTML Dasar</a>
 </nav>
 <!-- CSS ID Selector -->
 <div id="intro">
 <h1>Hello World</h1>
 <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman 
Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat 
adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML 
dan CSS.</p>
 <!-- CSS Class Selector -->
 <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
 </div>
</body>
</html>
```
![1](https://user-images.githubusercontent.com/56241285/114561331-ad837380-9c97-11eb-87a8-005a135e7073.png)
## Langkah 2
### Mendeklarasikan CSS Internal
```
<head>
 <title>CSS Dasar</title>
 <style>
 body {
 font-family:'Open Sans', sans-serif;
 }
 header {
 min-height: 80px;
 border-bottom:1px solid #77CCEF;
 }
 h1 {
 font-size: 24px;
 color: #0F189F;
 text-align: center;
 padding: 20px 10px;
 }
 h1 i {
 color:#6d6a6b;
 }
 </style>
</head>
```
![2](https://user-images.githubusercontent.com/56241285/114561722-03581b80-9c98-11eb-8ac8-cb2d64ed7775.png)
## Langkah 3 
### Menambahkan Inline CSS
```
<p style="text-align: center; color: #ccd8e4;">Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman 
Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat 
adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML 
dan CSS.</p>
```
![3](https://user-images.githubusercontent.com/56241285/114563052-436bce00-9c99-11eb-8c4a-536d68472ea3.png)
## Langkah 4
### Membuat CSS Eksternal
#### Buatlah file baru dengan nama style_eksternal.css
![4](https://user-images.githubusercontent.com/56241285/114569749-6f8a4d80-9c9f-11eb-8603-5b6f9321de81.png)
#### lalu masukan Coding 
```
nav {
    background: #20A759;
    color:#fff;
    padding: 10px;
    }
    nav a {
    color: #fff;
    text-decoration: none;
    padding:10px 20px;
    }
    nav .active, 
    nav a:hover {
    background: #0B6B3A;
    }
```
![5](https://user-images.githubusercontent.com/56241285/114569984-a52f3680-9c9f-11eb-8b8f-f8a510a723e8.png)
#### lalu masukan coding di bawah ke lab2_css_dasar.html
```
<head>
 <!-- menyisipkan css eksternal -->
 <link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
```
![6](https://user-images.githubusercontent.com/56241285/114570397-ff2ffc00-9c9f-11eb-9b31-9bc27766e6d3.png)
## Langkah 5
### Menambahkan CSS Selector 
```
/* ID Selector */
#intro {
background: #418fb1;
border: 1px solid #099249;
min-height: 100px;
padding: 10px;
}
#intro h1 {
text-align: left;
border: 0;
color: #fff;
}
/* Class Selector */
.button {
 padding: 15px 20px;
background: #bebcbd;
color: #fff;
display: inline-block;
margin: 10px;
text-decoration: none;
}
.btn-primary {
background: #E42A42;
}
```
![7](https://user-images.githubusercontent.com/56241285/114570912-6c439180-9ca0-11eb-8a65-66cd3f426132.png)
# TUGAS
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
- Saya bereksperimen menambahkan background dan mengubah warna pada button
![8](https://user-images.githubusercontent.com/56241285/115391636-e2e50f80-a209-11eb-9656-cad0afac82d4.png)
![9](https://user-images.githubusercontent.com/56241285/115391682-ec6e7780-a209-11eb-94da-355e43c9c186.png)
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya!
```
Pendeklarasian CSS elemen h1 mengubah tampilan seluruh elemen yang memiliki tag h1, jika #intro h1 hanya mengubah tampilan elemen h1 yang memiliki id #intro.
```
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
- jika mendeklarasikan CSS pada elemen yang sama namun isi deklarasi nya berbeda, maka semua deklarasi CSS tersebut akan ditampilkan.
![10](https://user-images.githubusercontent.com/56241285/115393213-a3b7be00-a20b-11eb-9c43-83812ef3397d.png)
![11](https://user-images.githubusercontent.com/56241285/115393233-a9150880-a20b-11eb-84dd-5d2c40555ff3.png)
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )
- Kedua deklarasi tersebut akan tampil
![12](https://user-images.githubusercontent.com/56241285/115394136-a9fa6a00-a20c-11eb-9746-23ecb31c3b03.png)
![13](https://user-images.githubusercontent.com/56241285/115394153-af57b480-a20c-11eb-91b7-a0942aee3c57.png)
