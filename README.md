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

Copy all the ```.nginx``` folder into your ```/home/web/mirror``` directory.

Demo: http://indexer.zvoid.net/

##### BEFORE
![before](http://indexer.zvoid.net/before.png)

##### AFTER
![after](http://indexer.zvoid.net/after.png)
