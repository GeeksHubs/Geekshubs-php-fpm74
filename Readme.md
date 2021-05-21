<h1 align="center">
 Docker File from php7.4  <br>
 (Laravel, Symfony, Wordpress, etc..)
</h1>

<p align="center">
    <img src="https://github.com/GeeksHubsAcademy/2020-geekshubs-media/blob/master/image/logo.png">	
</p>


![Packagist PHP Version Support](https://img.shields.io/badge/php-%5E7.2-blue)


Docker file for use in PHP Laravels support for php 7.2.
- Symfony
- Laravel
- PhpCake.
- Wordpress.
- Drupal.
- etc.




## 🚀 Installation
### Docker Hub.

From Docker Hub.

In your terminal execute this sentences
```terminal
docker pull geekshubs/geekshubs-php-fpm74
docker run -p 9000:9000 geekshubs/geekshubs-php-fpm74  
```
From Docker File.

In your terminal in same folder you down dockerfile execute this sentences.
```terminal
docker build -t geekshubs/geekshubs-php-fpm74 .
docker run -p 9000:9000  --name geekshubs_php74 geekshubs/geekshubs-php-fpm74 
```

## :arrow_forward: How to use.
In your web server to use this container add the proxy pass for example:.
### Apache.
```conf
ProxyPassMatch ^/(.*\.php(/.*)?)$ fcgi://geekshubs_php74:9000/var/www/html/public/$1
```

## :mag_right: Change log
Please see <a href="https://github.com/GeeksHubs/Geekshubs-php-fpm74/blob/master/changelog.md">CHANGELOG</a> for more information what has changed recently.



## :superhero_woman: Contribute.
Feel free to make as many pull requests as you think fit, because there are so many things to do, all help is welcome.

Here is a guide if you want to take a look(https://github.com/GeeksHubsAcademy/2020-geekshubs-convenio/blob/master/contributing.md)

If you find a bug, let us know <a href="https://github.com/GeeksHubs/Geekshubs-php-fpm74/issues">here</a> .

If you request a new  <a href ="https://github.com/GeeksHubs/Geekshubs-php-fpm74/issues"> feature</a>.

