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

Will setup demo for this shortly!
