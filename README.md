# subject-220511

![image](https://user-images.githubusercontent.com/1501327/167747277-ce78786f-1588-4a91-b9c1-7fa1fca7acaa.png)

## .htaccess
```
DirectoryIndex index.php
Options +Indexes
DirectoryIndex /index/files.php

RewriteEngine on
RewriteCond %{HTTPS} off
RewriteRule ^(.*)$ https://%{HTTP_HOST}%{REQUEST_URI} [R=301,L]
RewriteCond %{HTTP_HOST} ^www\.(.*) [NC]
RewriteRule ^ http://%1%{REQUEST_URI} [L,R=301]
```

## WinMarge( 改行コードを比較しない ) 
![image](https://user-images.githubusercontent.com/1501327/167749329-be8ed975-0a3c-4aaa-a525-d2d01708d8c0.png)
