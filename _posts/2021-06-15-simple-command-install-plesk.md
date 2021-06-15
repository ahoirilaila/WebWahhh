---
layout: post
title: Simple Command Install Plesk
summary: Cara mudah install Plesk Panel! 1 Baris kode, Duarrrr! Plesk terinstall
categories: HowTo
tags: 
- Plesk
- How To
comments: true
---

> Plesk is a commercial web hosting platform with a control panel that allows a server administrator to set up new websites, reseller accounts, e-mail accounts and DNS entries through a web-based interface.
> ** – Wikipedia**

Mudahnya, Plesk itu panel untuk melakukan pengaturan web hosting. Saat ini sudah banyak penyedia Hosting yang menggunakan Plesk Panel.

Apabila Kamu sudah memiliki VPS atau server sendiri dan ingin melakukan instalasi Plesk Panel bisa saja. Untuk instalasi Plesk bisa memasukkan 1 command, dan tunggu sampai selesai. Berikut Command nya,

<code> sh <(curl https://autoinstall.plesk.com/one-click-installer || wget -O - https://autoinstall.plesk.com/one-click-installer) </code>

Pastikan untuk menjalankan command diatas melalui user root. Setelah menjalankan tunggu instalasi sampai selesai.