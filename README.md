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

## WinMerge( 改行コードを比較しない ) 
![image](https://user-images.githubusercontent.com/1501327/167749597-1aaab791-0239-4c59-a2a9-e3f32e76e981.png)

## ローカル用
```
DirectoryIndex index.php
Options +Indexes
DirectoryIndex /index/files.php
```
