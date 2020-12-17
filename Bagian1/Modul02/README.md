# Instalasi Apache dan PHP di Windows
- Download [Apache](https://httpd.apache.org/download.cgi#apache24)
- Download [PHP](https://www.php.net/downloads.php)

## Configure Apache
Open file ```httpd.conf``` C:\apache24\conf),

Check DocumentRoot

``` DocumentRoot "C:/apache24/htdocs" ```

Change value in DirectoryIndex

``` DirectoryIndex index.php index.html ```

Add in the last text httpd.conf
```
LoadModule phpx_module "C:/PHP-5.5.5/php5apache2_4.dll"
AddHandler application/x-httpd-php .php

PHPIniDir "C:/PHP-5.5.5" 
```

## when i do this i use
Use PHP 5.5.5 and Apache24 httpd-2.4.6