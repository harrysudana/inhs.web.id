---
title: "Brew Update PHP Default Ke Versi 7.4"
date: 2019-12-02T23:39:54+08:00
draft: false
Tags: ["OctoberCMS", "PHP"]
---

Setelah melakukan update dan upgrade brew, tiba-tiba CMS yang berbasiskan OctoberCMS gagal untuk berjalan sempurna.

![error-ocotbercms-pada-php74](/img/error-ocotbercms-pada-php74.png)

Belum sempat review untuk update code terbaru dari team OctoberCMS, akhirnya coba kita install php versi 7.3 kembali.

`brew install php@7.3`

Kemudian, buat symbolic link untuk php73 agar bisa digunakan dengan command php73 di cli.

`cd /usr/local/bin/`

`ln -s php73 ../Cellar/php@7.3/7.3.12/bin/php`

untuk sementara menjalankan menggunakan php73 saja dulu.

`php73 artisan serve`
