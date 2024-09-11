# nik-validator
NIK Validator is a package to convert Indonesian citizenship identity number into usefull information. You just call the **parse** method and input NIK number in the parameter, then you will get the informations (without internet connection).



clone from https://github.com/irsyadulibad/nik-validator
## Usage
* Installation
```
composer require fariswidhi/nik-validator
```

* Example
```php
<?php
use Irsyadulibad\NIKValidator\Generator;
use Irsyadulibad\NIKValidator\Validator;

$nik = (new Generator())->generate();
$parsed = Validator::set($nik)->parse();

if($parsed->valid) {
    var_dump($parsed);
}
```
