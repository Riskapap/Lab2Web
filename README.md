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
```
