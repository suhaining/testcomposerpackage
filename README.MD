# FatSmallTools
github的学习，学习发布composer package

# 安装
确保PHP版本在7.0以上。

推荐通过[Composer](https://getcomposer.org/)进行安装

Composer的安装请参考官方配置。

安装好Composer后，在你的项目中创建一个 composer.json 文件：
```json
{
    "require": {
        "suhaining/testcomposerpackage": "*"
    }
}
```

然后在项目文件夹下执行:
```bash
$ composer install
```

之后添加autoloader:
```php
<?php
require "vendor/autoload.php";
```

使用方法如下：
```php
use SuNingTestComposerPackage\SuNing;


$suNingClass = new SuNing();
echo $suNingClass->test();
输出：
this is suning composer package test
#包的地址
https://packagist.org/packages/suhaining/testcomposerpackage
