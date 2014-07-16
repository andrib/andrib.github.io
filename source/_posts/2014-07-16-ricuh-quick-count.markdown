---
layout: post
title: "QuickCount - Kertas Paku Kotak"
date: 2014-07-16 16:14:10 +0700
comments: true
categories: nasionalism, Indonesia
---

2014 Juli 09 selesai sudah momen coblos coblosan pilpres, yang sebelumnya sudah sama-sama melakukan kampanye dengan semangat memperebutkan kursi nomor 1 dan 2 di Indonesia, ya kursi Presiden dan wakilnya. Dengan lancar KPU berhasil menyelenggarakan proses pemilihan seperti saat-saat sebelumnya, proses pemungutan suara di masing-masing TPS dipantau langsung oleh tim KPU dan para LSM bersama beberapa pihak publik lain yang sengaja hadir untuk melakukan pengambilan data (perkiraan) perhitungan yang digunakan sebagai data quick count yang saat ini diberitakan secara sporadis melalui media (terutama televisi), ricuh mewarnai proses perhitungan suara, tuding sana sini antar simpatisan dan tim sukses terjadi karena data quick count yang belum bisa dipastikan kebenarannya (memang bukan real count, hanya sampling) seharusnya tidak perlu terjadi karena sebenarnya secara resmi (berdasarkan UU), perhitungan suara pemilu hanya dilakukan oleh KPU dan akan resmi diumumkan hasilnya pada tanggal 22 Juli 2014.

KPU sebagai lembaga yang bertanggung jawab menyelenggarakan proses pemilihan suara setiap kali diadakan pemilu di Indonesia, sampai saat ini masih menggunakan cara konvensional (kertas + paku + kotak) yang dinilai masih cara efektif yang bisa dilakukan hingga saat ini, namun sayangnya metode konvensional seperti itu masih juga memiliki celah kecurangan dalam prosesnya, ditambahlagi kecepatan dalam mendistribusikan hasil suara di tiap daerah untuk dihitung secara terpusat membutuhkan effort yang luar biasa.

Pernahkah terpikir oleh KPU untuk melirik metode lain (selain kertas paku kotak) seperti dengan menggunakan bantuan teknologi misalnya, dengan teknologi KPU bisa membuat sistem pemilihan suara yang elbih efektif dan terukur baik dari sisi reliabilitas kemampuan hitung maupun keamanan data. Takut dicurangi dari sisi teknologi? hacker, cracker, script kiddies? Saya yakin sekaliber para pengkaji teknologi informasi di pemerintahan sudah sangat hebat dalam hal ini, jadi kenapa harus takut?

Dalam bayangan saya, dengan terintegrasinya data e-ktp yang selama ini sudah ada (entah benar atau tidak), bisa dibuatkan terminal TPS dengan peralatan multitouch screen berikut rfid ektp reader. Hanya ada 2 pihak yang terlibat dalam sistem ini, yaitu KPU dan penyelenggara e-ktp. Jaringan yang digunakan menggunakan enkripsi ssl 2048bit melalui vpn dari KPU/ektp ke masing-masing TPS, satu ektp id hanya bisa melakukan 1 kali otentikasi ke database ektp untuk mendapatkan token, dengan token unik tersebut maka pemilih dapat melakukan pilihan suara (yang diupdate ke data KPU) tanpa diketahui siapa identitasnya, pengukuran keberhasilannya adalah data jumlah otentikasi ektp harus match dengan jumlah suara yang tersimpan di KPU.


{% img center /images/img/coblos.jpg %}
