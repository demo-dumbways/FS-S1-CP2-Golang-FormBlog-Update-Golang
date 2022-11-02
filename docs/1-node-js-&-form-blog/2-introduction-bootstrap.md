---
sidebar_position: 2
---

# 2. Introduction Bootstrap

import useBaseUrl from '@docusaurus/useBaseUrl';

**Bootstrap** adalah kerangka kerja CSS yang sumber terbuka (Open Source) dan bebas untuk merancang situs web dan aplikasi web. Kerangka kerja ini berisi template desain berbasis HTML dan CSS untuk `tipografi, formulir, tombol, navigasi, dan komponen antarmuka lainnya`, serta juga ekstensi opsional JavaScript

## Instalasi Bootstrap

Bootstrap dapat digunakan didalam suatu project apabila telah dilakukan instalasi. Hanya saja maksud dari instalasi disini bukanlah seperti yang kita lakukan pada saat instalasi Node Js, melainkan menyediakan file - file css bootstrap kedalam project kita. Untuk melakukan hal tersebut, bisa dilakukan dengan 2 cara.

1. Instalasi Secara Offline
    Apabila ingin melakukan instalasi secara offline maka dapat melakukan tahapan berikut:
    - Download file bootstrap melalui laman resminya [getbootstrap.com](https://getbootstrap.com/docs/5.0/getting-started/download/)
    - Extract file bootstrap yang telah didownload ke dalam folder project yang menggunakan bootstrap
    
    File bootstrap yang didonwload akan berisikan 2 folder, yakni folder `CSS dan JS`. Folder CSS berisikan file - file css yang siap digunakan nantinya pada project, sedangkan folder JS berisikan script - script untuk mendukung styling CSS agar lebih interaktif. 

2. Instalasi Secara Online
    Apabila ingin melakukan instalasi bootstrap secara online maka akan lebih mudah, karena kita cukup menambahkan code pada file project. Code yang ditambahkan bertujuan untuk mengakses file `CSS dan JS Bootstrap` melalui `Content Delivery Network (CDN)`. **Content Delivery Network** adalah suatu teknologi yang memungkinkan kita mengakses data - data ataupun file dari sebuah website melalui jaringan internet secara lebih cepat.

    ```html 
    <!DOCTYPE HTML>
    <html>
        <head>
            <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" 
                    rel="stylesheet" 
                    integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" 
                    crossorigin="anonymous">

            <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" 
                    integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" 
                    crossorigin="anonymous"></script>
        </head>

        <body>
        </body>
    </html>
    ```


## Penggunaan Bootstrap

Apabila ingin melakukan instalasi bootstrap secara online maka akan lebih mudah, karena kita cukup menambahkan code pada file project. Code yang ditambahkan bertujuan untuk mengakses file `CSS dan JS Bootstrap` melalui `Content Delivery Network (CDN)`. **Content Delivery Network** adalah suatu teknologi yang memungkinkan kita mengakses data - data ataupun file dari sebuah website melalui jaringan internet secara lebih cepat.

Penggunaan bootrstrap yang diinstalasi secara offline maupun online tidak ada perbedaan. Kali ini kita aka mencoba membuat sebuah modal menggunakan template yang disediakan oleh bootstrap.
- Akses halaman template bootstrap  [getbootstrap.com/docs/5.1/components/modal/](https://getbootstrap.com/docs/5.1/components/modal/)
- copy salah satu template yang disediakan

<a class="btn-example-code" href="https://github.com/demo-dumbways/ebook-code-result-chapter-2-golang/blob/day1-1-introduction-bootstrap/index.html">
Contoh code
</a>

<br />
<br />

```html title="form-blog.hbs"
<!DOCTYPE HTML>
<html>

<head>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p"
        crossorigin="anonymous"></script>
</head>

<body>
    <!-- Button trigger modal -->
    <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
        Launch demo modal
    </button>

    <!-- Modal -->
    <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="exampleModalLabel">Modal title</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    ...
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
                    <button type="button" class="btn btn-primary">Save changes</button>
                </div>
            </div>
        </div>
    </div>
</body>

</html>
```

<img alt="image1" src={useBaseUrl('img/docs/image-1-0.png')} height="500px"/>

<br />
<br />

<div>
<a class="btn-demo" href="https://ebook-code-result-chapter-2-git-day1-0intr-893c86-demo-dumbways.vercel.app/">
Demo
</a>
</div>


        
