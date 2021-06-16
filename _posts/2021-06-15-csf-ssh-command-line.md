---
layout: post
title: CSF SSH Command Line
permalink: /csf-ssh-command-line/
summary: Cheat Sheet CSF Command Line biar nda salah ketik! Yahaha Hayuk
categories: Command
tags: 
- WHM
- cPanel
- Command
comments: true
---

CSF atau singkatan dari ConfigServer Firewall. Dilihat dari kepanjangannya saja sudah terbayang fungsi dari CSF itu sendiri. Untuk meningkatkan kemanan server berbasis Linux. Simple nya gitu, untuk lebih lengkapnya bisa cari di Google.com

Pada artikel ini saya membagikan SSH Command Line untuk penggunaan CSF itu sendiri. Untuk catatan saya sendiri juga, dan mungkin kalian ada yang mencari juga.

| Perintah             | Fungsi                                                   |
|----------------------|----------------------------------------------------------|
| csf -e               | Mengaktifkan CSF                                         |
| csf -x               | Menonaktifkan CSF                                        |
| csf -r               | Restart CSF                                              |
| csf -a [IP address]  | Allow IP dan menambahkan ke /etc/csf/csf.allow           |
| csf -td [IP address] | Block sementara IP, list ada di /var/lib/csf/csf.tempban |
| csf -tr [IP address] | Remove IP dari block sementara                           |
| csf -d [IP address]  | Block IP dan menambahkan ke /etc/csf/csf.deny            |
| csf -dr [IP address] | Remove IP dari Block                                     |
| csf -df [IP address] | Remove semua IP dari list Block /etc/csf/csf.deny        |
| csf -g [IP address]  | Mencari IP yang terblock di CSF                          |