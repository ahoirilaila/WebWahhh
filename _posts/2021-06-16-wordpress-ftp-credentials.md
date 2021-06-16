---
layout: post
title: Wordpress FTP Credentials
summary: Mengatasi FTP Credentials pada Wordpress ~
categories: wordpress HowTo
tags: 
- How To
- wordpress
comments: true
---

Jika pada saat melakukan instalasi Plugin dan tampil popup FTP credential silahkan tambahkan kode berikut di akhir file wp-config.php,

<code>
define('FS_METHOD','direct');
</code>

Setelah itu save file, dan dicoba kembali melakukan instalasi Pluginnya.