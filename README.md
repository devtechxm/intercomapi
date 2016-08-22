## Installation

Requires intercom-php v3.0.0

Using Composer:

The recommended way to install intercomsdk is through [Composer](https://getcomposer.org):

First, install Composer:

```
$ curl -sS https://getcomposer.org/installer | php
```

Next, install the latest intercomsdk:

```
$ php composer.phar require devtechxm/intercomsdk
```

Finally, you can include the files in your PHP script:

```php
require "vendor/autoload.php";
```

## Clients

```php
use Intercom\Api;

$intercom = new Api(appId, apiKey);
$client = $intercom->client;
```

## Users

```php
// Create/update a user
$client->users->create([
  "email" => "test@intercom.io"
]);
```
For More details visit [intercom reference](https://developers.intercom.io/reference) 
