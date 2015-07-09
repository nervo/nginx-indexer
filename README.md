Nginx Indexer
-------------
*Coded by Tuxy*

Nginx Indexer coded with HTML/CSS and using PNG 16x16 icons.

The ```ngx_http_addition_module``` required for this to work.

#### Config Nginx

```
server {
  listen 80;
  server_name mirror.domain.com;
  root /home/web/mirror;
  add_before_body /.nginx/header.html;
  add_after_body /.nginx/footer.html;
  autoindex on;
} #indexer
```

Copy ```.nginx``` folder into your ```/home/web/mirror``` directory.

Demo: http://indexer.zvoid.net/

#### BEFORE
![before](http://i.imgur.com/aSg9h5K.png)

#### AFTER
![after](http://i.imgur.com/aL3IVZ9.png)

#### Additional Icons
You're welcome to request additional icons for any mime-types in issue tracker.

Request Example Format:
 * Name: Executable
 * Extension: exe
 * Icon: 16x16px (imgur.com icon link)
 * Site: (official site or wiki page if any)

#### Supported Extensions

##### checksums
```
.sig, .asc, .pgp, .md5, .sha1, .sha256, MD5, SHA1, SHA256
```

##### compressed
```
.7z, .zip, .rar, .tar, .tar.gz, .tgz, .deb, .rpm, .iso, .bin, .cue
```

##### data storage
```
.csv, .json, .xml, .yaml, .yml, .sql, .sqlite, .ini, .reg
```

##### documents
```
.pdf, .chm, .djvu, .epub, .mobi, .txt, .rtf, .doc
```

##### information
```
CHANGELOG, INSTALL, COPYING, LICENSE, README, .nfo, .diz
```

##### media files
```
.avi, .flac, .flv, .gif, .jpeg, .jpg, .mkv, .mp3, .mp4, .psd, .png, .mov, .ra, .rv, .wav, .bmp
```

##### source code
```
.h, .c, .cpp, .css, .go, .htm, .html, .class, .java, .js, .lua, .pl, .php, .nim, .rlib, .rs, .less, .py, .rb, .sh
```
