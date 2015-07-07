Nginx Indexer
-------------
*Coded by Tuxy*

#### Config Nginx

```
server {
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
