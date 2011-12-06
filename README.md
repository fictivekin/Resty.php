# Resty.php

A simple PHP library for doing RESTful HTTP stuff. Does *not* require the curl extension.

## Example

```php
require __DIR__."/Resty.php";

$resty = new Resty();
$resty->enableDebugging(true);
$resty->setBaseURL('https://gimmebar.com/api/v0/');
$resp = $resty->get('public/assets/funkatron');
print_r($resp);
```