---
sidebar_position: 4
---

# 4. Creating Form Blog

import useBaseUrl from '@docusaurus/useBaseUrl';

Sama halnya dengan pembuatan navbar, untuk membuat form blog kita juga akan memanfaatkan template dan class - class yang disediakan oleh bootstrap.

<br/>
<a class="btn-example-code" href="https://github.com/demo-dumbways/ebook-code-result-chapter-2-golang/blob/day1-3-form-blog/form-blog.html">
Contoh code
</a>
<br/>
<br/>

```html {30-47} title="form-blog.html"
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

  <form class="form-container">
    <h1>Create Post Blog</h1>
    <div>
      <label for="input-title" class="form-label">Title</label>
      <input id="input-title" name="title" class="form-control" />
    </div>
    <div>
      <label for="input-content" class="form-label">Content</label>
      <textarea id="input-content" name="content" class="form-control"></textarea>
    </div>
    <div>
      <label for="input-image" class="form-label">Upload Image</label>
      <input class="form-control" type="file" id="input-image">
    </div>
    <div class="d-flex justify-content-end">
      <button class="btn">Post Blog</button>
    </div>
  </form>

</body>
</html>
```

Pada bagian form pun kita mengkombinsikan bootstrap dengan css external yang kita tuliskan padaa `style.css`.  Komponen dan class yang dilakukan styling tambahan adalah:
- form-container
- h1
- label
- input
- textarea
- select
- button

Akses hasil refactor code menggunakan bootstrap untuk styling pada file index, contact, blog, dan blog detail pada button berikut
   <a class="btn-example-code" href="https://github.com/demo-dumbways/ebook-code-result-chapter-2-golang/tree/day1-4-full-code">
   Full code
   </a>

   <br />   
   <br />   


<img alt="image1" src={useBaseUrl('img/docs/image-2-1.png')} height="500px"/>

<br />
<br />

<div>
<a class="btn-demo" href="https://ebook-code-result-chapter-2-git-day1-2navbar-demo-dumbways.vercel.app/">
Demo
</a>
</div>
   
   