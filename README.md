# CriticalImpact

A PHP library for working w/ the [CriticalImpact API](http://ci.criticalimpact.com/api8/).

## Install

Normal install via Composer.

## Usage

```php
use Travis\CriticalImpact;

// add subscriber
$response = CriticalImpact::run('subscriber', 'post', $apikey, [
	'listId' => 'LISTID',
	'email' => 'EMAIL',
	'firstname' => 'FIRST',
	'lastname' => 'LAST',
	'unsubscribe' => 0, // 0=subscribe, 1=unsubscribe
]);
```

For more information, consult the [API Docs](http://ci.criticalimpact.com/api8/) page.