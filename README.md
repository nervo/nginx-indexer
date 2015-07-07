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
