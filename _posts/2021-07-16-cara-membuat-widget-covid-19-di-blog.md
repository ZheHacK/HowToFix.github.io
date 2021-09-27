---
layout: post
title: Cara membuat Widget Status COVID 19 Indonesia
subtitle:  Cara membuat Widget Status COVID 19 Indonesia
cover-img: https://telegra.ph/file/c7b73b2c0b54740ee0154.png
thumbnail-img: https://telegra.ph/file/c7b73b2c0b54740ee0154.png
tags: [html, JavaScript, css]
comments: true
---


Cara pemasangannya cukup simple, saya coba menjelaskan cara pemasangan di wordpress dan blogspot.

Pasang widget kawal corona di WordPress
Untuk website yang dibangun dengan wordpress, kita dapat masuk ke halaman Tampilan, lalu masuk ke menu Widget.


 
Setelah itu, kita tambahkan widget HTML Khusus kedalam sidebar. Lalu pada kolom isi di widget HTML Khusus kita tambahkan script dibawah ini

<script src="https://gist.github.com/MadeWiguna/aee3f012c1880f6b4cb3c5baa7260335.js"></script>



Pasang widget kawal corona di Blogger / Blogspot
Untuk memasang widget kawal corona di Blogger/Blogspot kalian dapat masuk ke halaman Tata Letak, lalu klik tombol "Tambahkan Widget". Saat muncul popup, kalian pilih menu HTML/JavaScript 


<script src="https://gist.github.com/MadeWiguna/aee3f012c1880f6b4cb3c5baa7260335.js"></script>


## Demo

<div id="MadeWiguna-covid"></div>
<script>
  var f = document.createElement("iframe");
  f.src = "https://madewiguna.netlify.app/proyek/covid.html";
  f.width = "100%";
  f.height = 380;
  f.scrolling = "no";
  f.frameBorder = 0;
  var rootEl = document.getElementById("MadeWiguna-covid");
  console.log(rootEl);
  rootEl.appendChild(f);
</script>


<script async src="https://comments.app/js/widget.js?3" data-comments-app-website="EJ5VGbXx" data-limit="100"></script>
