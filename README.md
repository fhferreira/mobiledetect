# MobilDetect package for Laravel

[![Build Status](https://travis-ci.org/larapack/laravel-mobiledetect.svg)](https://travis-ci.org/larapack/laravel-mobiledetect)
[![Total Downloads](https://poser.pugx.org/larapack/mobiledetect/downloads.svg)](https://packagist.org/packages/larapack/mobiledetect)
[![Latest Stable Version](https://poser.pugx.org/larapack/mobiledetect/v/stable.svg)](https://packagist.org/packages/larapack/mobiledetect)
[![Latest Unstable Version](https://poser.pugx.org/larapack/mobiledetect/v/unstable.svg)](https://packagist.org/packages/larapack/mobiledetect)
[![License](https://poser.pugx.org/larapack/mobiledetect/license.svg)](https://packagist.org/packages/larapack/mobiledetect)

### Installation

First add the package to your composer by running command `composer require larapack/mobiledetect 1.*` or by adding the following code to `composer.json` followed by running the command `composer update`:
```
{
    "require": {
        "larapack/mobiledetect": "1.*"
    }
}
```

Add the alias to the aliases in your `app/config/app.php`:
```
'aliases' => array(
    // ...
    'MobileDetect' => 'Larapack\MobileDetect\MobileDetect',
)
```

### Usage

The following examples assume you use the MobileDetect class name as alias, but the packages is namespaced so you can name the facade as you wish.

```
$detect = MobileDetect;

if ($detect->isMobile()){
  // this is a mobile
}
else if ($detect->isTablet()){
  // this is a tablet
}

if ($detect->isIE()){
  // this is IE -.-'
}
```

More examples on http://mobiledetect.net/
