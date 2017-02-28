# Configure of htaccess

## Redirect all
```
RewriteEngine on
Redirect permanent / [TO]
```

## Basic 
```
RewriteEngine on
RewriteBase /
RewriteRule [FROM] [TO] [R=301,L]
```

## Directory
```
RewriteEngine on
RewriteBase /
RewriteRule ^[FROM_DIR]/(.*)$ /[TO_DIR]/$1 [R=301,L]
```

## Dtop search engines crowling
```
SetEnvIf User-Agent "Googlebot" shutout
SetEnvIf User-Agent "Slurp" shutout
SetEnvIf User-Agent "msnbot" shutout
order Allow,Deny
Allow from all
Deny from env=shutout
```
or use `robots.txt`
