---
layout: post
title: "Ghost - Platform Blog berbasis nodejs"
date: 2014-04-06 13:30:50 +0700
comments: true
categories: platform, blog-engine, nodejs
---



[Ghost](http://ghost.org/) merupakan platform blog sederhana dan cepat berbasis node.js, dibuat khusus sebagai *blog publishing engine*, dirancang dengan baik dan terstruktur serta memiliki kendali kustomisasi penuh bagi developer untuk mengubah isi konten, mengubah tampilan dengan mudah (membuat *template* desain sendiri) atau bahkan membuat modul program node.js tersendiri, [Ghost](http://ghost.org/) dibuat sepenuhnya terbuka (*Open Source* ). 


<p align='center'>
{% img left /images/img/ghost.png 350 350 'image' 'images' %}
</p>

Seperti *blog publishing engine* pada umumnya, [Ghost](http://ghost.org/) memiliki alur penggunaan aplikasi web yang sama, hanya saja sedikit berbeda pada modul *content management system* atau sering disebut sebagai *dashboard* pada *engine blog*, yaitu menggunakan *markdown* sebagai fungsi edit post, yang memudahkan web developer untuk tidak tergantung kepada wysiwyg editor berbasis javascript yang konvensional seperti ckeditor dan lainnya.

[Ghost](http://ghost.org/) "berjalan" di atas framwork node.js sepenuhnya, memiliki berbagai *driver* database untuk digunakan seperti postgre dan mysql yang tergolong *relational database*, selain itu Ghost juga mendukung penggunaan **NoSQL** database seperti MongoDB dan lainnya. Bagi para developer web yang terbiasa menggunakan **LAMP Stack**, mungkin sudah saatnya mulai mencoba beralih stack yang berbeda seperti node.js dalam membuat sebuah website, sebagian orang menganggap node.js ini masih baru dan belum bisa dikategorikan sebagai framework web development dalam skala *enterprise*, tetapi perlu dipertimbangkan bahwa node.js ini membuat proses development lebih cepat dan menghasilkan aplikasi web yang *scalable* :)

