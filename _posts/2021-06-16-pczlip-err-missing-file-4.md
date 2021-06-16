---
layout: post
title: PCLZIP_ERR_MISSING_FILE (-4)
summary: Error temporary wordpress yang kadang menyebalkan!
categories: wordpress HowTo
tags: 
- How To
- wordpress
comments: true
---

Setiap melakukan instalasi plugin pada wordpress akan membuat file sementara atau temporary yang disimpan pada folder /tmp/.

Jika pada saat melakukan instalasi terdapat error, 
<code>
Installation failed: The package could not be installed. PCLZIP_ERR_MISSING_FILE (-4) : Missing archive file '/tmp/classic-editor.1.5-a61K01.tmp'
</code>

Pesan error tersebut karena wordpress tidak bisa menulis file sementara atau temporary pada instalasi.

1. Buat folder tmp/ di wp-content (/wp-content/tmp/).

2. Edit file wp-config.php dan cari code berikut,

<code>
if ( !defined('ABSPATH') )
    define('ABSPATH', dirname(__FILE__) . '/');
</code>

3. Setelah itu tambahkan kode berikut dibawahnya,

<code>
/** Specify wordpress temp dir */
define('WP_TEMP_DIR', ABSPATH . 'wp-content/temp');
</code>

Coba lakukan instalasi kembali.