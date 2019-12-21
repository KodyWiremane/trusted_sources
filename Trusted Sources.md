### <center>**Kody Wiremane's**</center>

# <center>**TRUSTED SOURCES**</center>

## **Abstract**

This is my own first organized attempt in building a reference base of programming tools and libraries that I can trust and use in software development. As my conserns currently revolve around PHP, it shall begin as PHP-centric.

Published under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

## **Methodology**

I declare some entities I believe I can trust, as trust anchors ("Trust Axioms"). Those are software products, or developers (either individual or collective), or integrators, that/who can act as a trust authority.

If a Trust Axiom uses a tool/library, it implies trust. Assuming the Axiom is competent, I can trust the tool/library as well. I write it down ("Trust Theorems") as a trusted entity's name, accompanied with references to its trustees.

Of course, such an approach has its downsides… Though it has certain advantages over manual analysis of source codes, or lack of any analysis at all.

So, here go

## **Trust Axioms**

### **`Amazon`**

Tag: amazon<br/>
Link: https://www.amazon.com/<br/>
Info: A big company focusing on e-commerce, cloud computing, digital streaming, and artificial intelligence. They have their own software, which potentially uses \[trusted] third-party libraries.

### **`Debian`**
Tag: debian<br/>
Link: https://www.debian.org/<br/>
Info: A GNU/Linux distribution maintained by the Debian Project. The oldest Linux-based OS. If they include software into their repositories, I believe I can trust it.

### **`Google`**
Tag: google<br/>
Link: https://www.google.com/<br/>
Info: A big company that specializes in Internet-related services and products, which include online advertising technologies, a search engine, cloud computing, software, and hardware. They have their own software, and it defenitely trusts come third-party stuff.

### **`ICANN`**
Tag: icann<br/>
Link: https://www.icann.org/<br/>
Info: A nonprofit organization responsible for coordinating the maintenance and procedures of several databases related to the namespaces and numerical spaces of the Internet, ensuring the network's stable and secure operation. Not much the software type, probably, though an authority.

### **`IETF`**
Tag: ietf<br/>
About: Internet Engineering Task Force is the premier Internet standards body, developing open standards through open processes. Again, not much about palpable software, though an authority.<br/>
Link: https://www.ietf.org/

### **`Linux`**
Tag: linux<br/>
Link: https://www.kernel.org/<br/>
Info: A free and open-source, monolithic, Unix-like operating system kernel, created by Linus Torvalds.

### **`Microsoft`**
Tag: microsoft<br/>
Link: https://www.microsoft.com/<br/>
Info: A big company; among other things, the creator of OS Windows, Xbox game console, and Azure cloud services.

### **`Mozilla`**
Tag: mozilla<br/>
Link: https://www.mozilla.org/<br/>
Info: A free software community founded in 1998 by members of Netscape. The Mozilla community uses, develops, spreads and supports Mozilla products, thereby promoting exclusively free software and open standards, with only minor exceptions.

### **`Tumblr`**
Tag: tumblr<br/>
Link: https://www.tumblr.com/<br/>
Info: An American microblogging and social networking website. They have dev docs at https://www.tumblr.com/developers.

## **Trust Theorems**

### **`Composer`**

Tag: composer<br/>
Trustees:

* [#debian](#debian) (https://packages.debian.org/buster/composer → https://getcomposer.org/)

About: Package manager for PHP.<br/>
Link: https://getcomposer.org/

### **`Drupal`**

Tag: drupal
Trustees:

* [#debian](#debian) (https://packages.debian.org/stretch/drupal7 → https://www.drupal.org/)
* [#symfony](#symfony) (https://symfony.com/projects → https://symfony.com/projects/drupal → https://drupal.org/)

About: PHP CMS.<br/>
Link: https://www.drupal.org/

### **`Drush`**

Tag: drush<br/>
Trustees:

* [#drupal](#drupal) (https://www.drupal.org/node/1791676 → https://github.com/drush-ops/drush → https://docs.drush.org/en/master/install/ → https://packagist.org/packages/drush/drush)

About: A command line shell and scripting interface for Drupal, by Arto Bendiken.<br/>
Link: https://github.com/drush-ops/drush<br/>
Link: https://packagist.org/packages/drush/drush

### **`google/apiclient`**

Tag: gapi-client<br/>
Trustees:

* [#google](#google) (https://developers.google.com/drive/api/v3/downloads?hl=en → https://github.com/googleapis/google-api-php-client → https://packagist.org/packages/google/apiclient)
* [#debian](#debian) (https://packages.debian.org/jessie/php/php-google-api-php-client → https://code.google.com/archive/p/google-api-php-client/ → https://github.com/googleapis/google-api-php-client)

About: Google API PHP client library<br/>
Link: https://packagist.org/packages/google/apiclient

### **`Guzzle HTTP Client`**

Tag: guzzlehttp<br/>
Trust:

* [#gapi-client](#google/apiclient) (code dependency)

About: PHP HTTP client library<br/>
Link: https://packagist.org/packages/guzzlehttp/guzzle

### **`Joomla`**

Trustees:

* [#symfony](#symfony) (https://symfony.com/projects → https://symfony.com/projects/joomla → https://www.joomla.org/)

About: PHP CMS<br/>
Link: https://www.joomla.org/

### **`JSON Schema`**

Tag: json-schema<br/>
Trustees:

* [#ietf](#ietf) (https://tools.ietf.org/html/draft-handrews-json-schema-01 → https://json-schema.org/)

About: Validation standard for JSON<br/>
Link: https://json-schema.org/

### **`Laravel`**

Tag: laravel<br/>
Trustees:

* [#symfony](#symfony) (https://symfony.com/projects → https://symfony.com/projects/laravel → https://laravel.com/)

About: PHP Framework<br/>
Link: https://laravel.com/

### **`monolog/monolog`**

Tag: monolog<br/>
Trustees:
* [#debian](#debian) (https://packages.debian.org/buster/php-monolog → https://github.com/Seldaek/monolog → https://packagist.org/packages/monolog/monolog)
* [#gapi-client](#google/apiclient) (https://packagist.org/packages/google/apiclient → https://packagist.org/packages/monolog/monolog)

About: PHP logging library<br/>
Link: https://packagist.org/packages/monolog/monolog

### **`myclabs/deep-copy`**

Trustees:

* [#phpunit](#phpunit) (https://packagist.org/packages/phpunit/phpunit → https://packagist.org/packages/myclabs/deep-copy)

About: Create deep copies (clones) of your objects<br/>
Link: https://packagist.org/packages/myclabs/deep-copy

### **`NodeJS`**

Trustees:

* [#debian](#debian) (https://packages.debian.org/buster/nodejs → https://nodejs.org/)

About: Event-based V8 JS engine<br/>
Link: https://nodejs.org/

### **`NPM`**

Trustees:

* [#debian](#debian) (https://packages.debian.org/buster/npm → https://docs.npmjs.com/ → https://www.npmjs.com/)

About: Package manager for NodeJS<br/>
Link: https://www.npmjs.com/

### **`OAuth`**

Trustees: [#ietf](#ietf) (https://tools.ietf.org/html/rfc5849 → https://oauth.net/)

About: Network auth protocol<br/>
Link: https://oauth.net/

### **`Opis`**
Trustees:

* [#laravel](#laravel) (https://packagist.org/packages/laravel/framework → https://packagist.org/packages/opis/closure)
* [#yii](#yii) (https://www.yiiframework.com/ → https://github.com/yiisoft → https://github.com/yiisoft/yii2-debug → composer.json → https://packagist.org/packages/opis/closure)

About: «High-quality PHP software — A fantastic collection of well crafted, developer-focused, open-source libraries»<br/>
Link: https://opis.io/

### **`Packagist`**

Trustees:

* [#composer](#composer) (https://getcomposer.org/ → https://packagist.org/)

About: Composer's online repository<br/>
Link: https://packagist.org/

### **`PHP`**

Trustees:

* [#debian](#debian) (https://packages.debian.org/buster/php → https://packages.debian.org/buster/php7.3 → https://www.php.net/)

About: Server-side scripting language<br/>
Link: https://www.php.net/

### **`PHP-FIG`**

Trustees:

* [#psr-log](#psr/log) (well, it's their package)
* [#monolog](#monolog/monolog) (trusts the package above)

About: PHP Framework Interop Group<br/>
Link: https://www.php-fig.org/

### **`PHP-JWT`**

Trustees:

* [#gapi-client](#google/apiclient) (https://packagist.org/packages/google/apiclient → https://packagist.org/packages/firebase/php-jwt)

About: A simple library to encode and decode JSON Web Tokens (JWT) in PHP, conforming to RFC 7519.<br/>
Link: https://packagist.org/packages/firebase/php-jwt

### `phpseclib/phpseclib`

Trustees:

* [#laravel](#laravel) (https://packagist.org/packages/laravel/framework → https://packagist.org/packages/phpseclib/phpseclib)
* [#gapi-client](#google/apiclient) (https://packagist.org/packages/google/apiclient → https://packagist.org/packages/phpseclib/phpseclib)

About: Pure-PHP implementations of RSA, AES, SSH2, SFTP, X.509 etc.<br/>
Link: https://packagist.org/packages/phpseclib/phpseclib

### **`PHPUnit`**

Tag: phpunit<br/>
Trustees:

* [#debian](#debian) (https://packages.debian.org/buster/phpunit → https://phpunit.de/ → https://packagist.org/packages/phpunit/phpunit)

About: PHP testing framework<br/>
Link: https://phpunit.de/<br/>
Link: https://packagist.org/packages/phpunit/phpunit

### **`psr/log`**

Tag: psr-log
Trustees:

* [#monolog](#monolog/monolog)<br/>

About: Common interface for logging libraries<br/>
Link: https://packagist.org/packages/psr/log

### **`Symfony`**

Tag: symfony<br/>
Trustees:

* [#debian](#debian) (https://packages.debian.org/buster/php-symfony → https://symfony.com/)

About: PHP framework; also refers to CakePHP, Zend Express, Magento, and others [here](https://symfony.com/projects)<br/>
Link: https://symfony.com/

### **`The League`**
Tag: league<br/>
Trustees:

* [#drush](#drush) (https://packagist.org/packages/drush/drush → https://packagist.org/packages/league/container)
* [#tumblr](#tumblr) (https://packagist.org/packages/tumblr/tumblr#dev-janicelee/integrate-library → https://packagist.org/packages/league/oauth2-client)

About: The League of Extraordinary Packages<br/>
Link: https://thephpleague.com/

### **`Yii`**

Tag: yii<br/>
Trustees:

* [#symfony](#symfony) (https://symfony.com/projects → https://symfony.com/projects/yii → https://www.yiiframework.com/)

About: PHP framework<br/>
Link: https://www.yiiframework.com/