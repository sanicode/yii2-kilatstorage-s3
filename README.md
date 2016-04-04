Yii2 KilatStorage S3
====================
This class is a standalone S3 REST implementation for PHP 5.2.x (using CURL), that supports large file uploads and doesn’t require PEAR.

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist sanicode/yii2-kilatstorage-s3 "*"
```

or add

```
"sanicode/yii2-kilatstorage-s3": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

```php
<?php 
    use sanicode\KilatStorageS3\S3;
    $s3 = new S3($accessKey, $secretKey);
    //put object
    $s3->putObjectFile(...)
    //delete object
    $s3->deleteObject(...)
?>
```
