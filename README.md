alifattahi/jdf
======

Laravel 4 Persian jalali date

<a name="installation"></a>
## Installation

In the `require` key of `composer.json` file add the following

```yml
    "alifti/jdf": "dev-master"
```

Run the Composer update comand

    $ composer update

In your `config/app.php` add `'Alifti\jdf\jdfServiceProvider'` to the end of the `$providers` array

```php
    'providers' => array(

        'Illuminate\Foundation\Providers\ArtisanServiceProvider',
        'Illuminate\Auth\AuthServiceProvider',
        ...
        'Alifti\Jdf\JdfServiceProvider',

    ),
```

<a name="basic-usage"></a>
## Basic Usage
## Examples ##

Some Examples (based on examples provided by Sallar)

```php
// Current date time
$date = jdf::jdate('H:i:s Y/m/d');

// current date time in unix time format
$date = jdf::jmktime();

// or create your jalali unix tiem format 
$date = jdf::jmktime($h,$m,$s,$jm,$jd,$jy);
```

Persian guide for all methods in this package : [Persian guide](http://jdf.scr.ir/rahnama/)

## License ##
- This package is created based on [jdf](http://jdf.scr.ir) 
- [Jalali (Shamsi) DateTime](https://github.com/alifattahi/jdf) class included in the package is created by [Ali Fattahi] and is released under the MIT License. 
- This package was created by [Ali Fattahi] and is released under the MIT License.
