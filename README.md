## Laravel Word v1.0.0 - in progres (refactoring from EXCEL to WORD)  

[<img src="http://www.maveius.pl/img/word_banner.png"/>](http://www.maveius.pl/laravel-word/docs)

Laravel Word brings the power of PHPOffice's PHPWord to Laravel 4 and 5 with a touch of the Laravel Magic. It includes features like: importing Word and RTF to collections, exporting models, array's and views to Word, importing batches of files and importing a file by a config file.

- Import into Laravel **Collections**
- Export **Blade views** to Word and RTF with optional CSS styling
- **Batch** imports
- A lot of optional **config settings**
- Easy **cell caching**
- Chunked importer
- WordFile method injections (Laravel ~5.0)
- Editing existing Word files
- **Advanced import** by config files
- and many more...

---

```php
Word::create('Laravel Word', function($word) {

    $excel->section('Word section', function($section) {

        $sheet->setOrientation('landscape');

    });

})->export('doc');
```

---

[![Build Status](https://travis-ci.org/Maatwebsite/Laravel-Excel.svg?branch=master)](https://travis-ci.org/Maatwebsite/Laravel-Excel)
[![Latest Stable Version](https://poser.pugx.org/maatwebsite/excel/v/stable.png)](https://packagist.org/packages/maatwebsite/excel) [![Total Downloads](https://poser.pugx.org/maatwebsite/excel/downloads.png)](https://packagist.org/packages/maatwebsite/excel)  [![License](https://poser.pugx.org/maatwebsite/excel/license.png)](https://packagist.org/packages/maatwebsite/excel)
[![Monthly Downloads](https://poser.pugx.org/maatwebsite/excel/d/monthly.png)](https://packagist.org/packages/maatwebsite/excel)
[![Daily Downloads](https://poser.pugx.org/maatwebsite/excel/d/daily.png)](https://packagist.org/packages/maatwebsite/excel)

#Installation

Require this package in your `composer.json` and update composer. This will download the package and PHPExcel of PHPOffice.

```php
"maatwebsite/excel": "~1.2.1"
```

After updating composer, add the ServiceProvider to the providers array in `app/config/app.php`

```php
'Maatwebsite\Excel\ExcelServiceProvider',
```

You can use the facade for shorter code. Add this to your aliases:

```php
'Excel' => 'Maatwebsite\Excel\Facades\Excel',
```

The class is bound to the ioC as `excel`

```php
$excel = App::make('excel');
```

# Documentation

The complete documentation can be found at: [http://www.maatwebsite.nl/laravel-excel/docs](http://www.maatwebsite.nl/laravel-excel/docs)

# Contributing

**ALL** bug fixes should be made to appropriate branch (e.g. `1.2` for 1.2.* bug fixes). Bug fixes should never be sent to the `master` branch.

More about contributing can be found at: [http://www.maatwebsite.nl/laravel-excel/docs/getting-started#contributing](http://www.maatwebsite.nl/laravel-excel/docs/getting-started#contributing)

# License

This package is licensed under LGPL. You are free to use it in personal and commercial projects. The code can be forked and modified, but the original copyright author should always be included!
