---
sidebar_position: 3
---

# 3. Creating Navbar

import useBaseUrl from '@docusaurus/useBaseUrl';

Sebelum kita membuat form blog pada study case, kita akan membuat navigation bar (navbar) terlebih dahulu. Pada chapter 1 kita membuat navbar secara manual, kali ini kita akan membuat navbar menggunakan template navbar yang telah disediakan oleh bootstrap.

Hal pertama yang kita lakukan adalah memuat bootstrap.css menggunakan `Content Delivery Network (CDN)`. **Content Delivery Network** adalah layanan jaringan pengantaran konten untuk publik.

<br />

```html {5-6} title="form-blog.html"
<!DOCTYPE html>
<head>
  <title>Blog Form With Bootstrap</title>
  <link rel="stylesheet" href="/public/style.css">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet"
    integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
</head>
<body>
</body>
</html>
```
Setelah kita memuat bootstrap.css menggunakan CDN, kita tambahkan template navbar yang telah disediakan oleh bootstrap dan kita customize menu - menu yang akan digunakan nantinya sesuai study case.

<br/>
<a class="btn-example-code" href="https://github.com/demo-dumbways/ebook-code-result-chapter-2-golang/blob/day1-2-creating-navbar/form-blog.html">
Contoh code
</a>
<br/>
<br/>

```html {9-28} title="form-blog.html"
<!DOCTYPE html>
<head>
  <title>Blog Form With Bootstrap</title>
  <link rel="stylesheet" href="/public/style.css">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet"
    integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
</head>
<body>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-lg">
      <a class="navbar-brand me-5" href="index.html">
        <img src="/public/assets/logo.png" alt="logo" />
      </a>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link" href="index.html">Home</a>
          </li>
          <li class="nav-item">
            <a href="blog.html" class="nav-link list-active">Blog</a>
          </li>
        </ul>
      </div>
      <div class="d-flex contact-me">
        <a href="contact.html"> Contact Me </a>
      </div>
    </div>
  </nav>
</body>
</html>
```

<img alt="image1" src={useBaseUrl('img/docs/image-1-2.png')} height="500px"/>

<br />
<br />

<div>
<a class="btn-demo" href="https://ebook-code-result-chapter-2-git-day1-1cdn-demo-dumbways.vercel.app/form-blog.html">
Demo
</a>
</div>

<br/>


Bootstrap juga bisa kita kombinasikan menggunakan css yang kita tuliskan sendiri, pada bagian `contact me` kita menggunakan/menambahan `class contact-me` yang styling nya kita tuliskan pada file `style.css`