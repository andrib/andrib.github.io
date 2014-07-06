---
layout: post
title: "Layanan SMTP Relay Berbayar"
date: 2014-04-10 13:10:10 +0700
comments: true
categories: system, mailserver, 3rdparty
---


Komunikasi email sebuah aplikasi memegang peranan yang sangat penting dan tidak dapat diabaikan begitu saja tentang reliabilitasnya, khususnya pada aplikasi layanan publik yang  dibuat untuk digunakan oleh pengguna umum secara global.

Sebagai contoh, pada sebuah aplikasi web, pada fungsi registrasi pengguna membutuhkan email sebagai alat untuk validasi akun pengguna, sebagai media notifikasi bagi pengguna, atau juga digunakan sebagai *mailing list* dalam aplikasi, tetapi apa yang terjadi jika semua email yang dikirim tidak terlihat dalam *inbox* para recipients? Tentunya bukan merupakan alasan yang baik dalam membentuk layanan dari aplikasi, jika kita pernah mengatakan kalimat "*coba cek spam box anda..*" kepada *recipients* dari aplikasi kita :)

Dalam lingkup sistem administrasi baik server-server berbasis linux atau lainnya, biasanya memiliki kendala pada sistem MTA (*Mail Transfer Agent*) pada mail server, seperti blacklist ip, whitelist ip, spam scores, spam complaints, atau konfigurasi server mail yang buruk, yang menyebabkan setiap email yang terkirim dari mail server tersebut dianggap SPAM oleh banyak mail server global, terutama penyedia layanan besar seperti yahoo dam google.


Banyak hal/persayaratan sebuah mail server yang kita buat dapat memiliki reputasi sending yang baik dalam skala global, dan hal tersebut membutuhkan waktu lama, khususnya dalam reputasi domain sender, domain-domain baru yang kita gunakan bisa saja akan tetap dianggap SPAM walaupun sudah memiliki mail server yang terkonfigurasi dengan baik.


Solusi sementara yang efektif bagi bisnis adalah dengan tetap menjalankan komunikasi email dari aplikasi dengan menggunakan layanan *smtp relay* berbayar, dengan cara ini aplikasi yang mengirimkan email melalui MTA harus melakukan metode relay ke MTA milik layanan smtp relay berbayar yang digunakan, dengan cara tersebut email yang terkirim melalui aplikasi memiliki garansi terkirim dengan baik ke seluruh tujuan recipients.

Berikut ini adalah beberapa layanan smtp relay berbayar yang dapat digunakan:

* [Postmark](http://postmarkapp.com/)
* [Amazon SES](http://aws.amazon.com/ses/)
* [Sendgrid](http://sendgrid.com/)
* [SocketLabs](http://socketlabs.com/)
* [MailJet](http://www.mailjet.com/)
* [Elastic Mail](http://www.elasticemail.com/)
* [smtp2go](http://www.elasticemail.com/)


Dari beberapa layanan diatas yang pernah saya coba, hanya postmark dan smtp2go, postmark adalah layanan kedua setelah saya gagal pada smtp2go :)

Kedua layanan sebenarnya ini cukup baik, smtp2go sangat mudah dalam proses instalasi, hanya saja smtp2go memiliki peraturan yang terlalu *strict* dalam masalah spam complaints dan reputasi akun kita (berhubungan dengan pola kirim email aplikasi), yang akhirnya jadi menyebalkan :)

<br />
{% img center /images/img/postmark.png %}



[Postmark](http://postmarkapp.com/) memiliki kelebihan lain dalam masalah perhitungan sewa layanan, yaitu menggunakan *credits* untuk mengirim email, jika kita memiliki 1000 credit, maka mail server kita bisa menggunakan relay sebanyak 1000 email terkirim. Pricing credits yang diberikan juga cukup murah, saat ini $7.5 per 1000 credit. Metode pricing menggunakan *credits* ini dinilai cocok bagi startup yang sebenarnya belum membutuhkan terlalu banyak komunikasi email pada tahap awal, tentunya tidak cocok jika menggunakan layanan smtp relay yang memiliki *bulk sending quota* dalam waktu yang ditentukan baik *annually* atau *monthly*
