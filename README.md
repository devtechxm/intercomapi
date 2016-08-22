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
```

## Users

```php
// Get a user	
	try 
    {
    		$client = $intercom->client;
    		//same as intercom-php sdk
		$response = $client->users->getUsers(["email" => "nouser@intercom.io"]);
	}
    catch (Exception $e) 
    {
    	$response = $intercom->parseExceptionError($e);
    }
    
    echo '<pre>';
    print_r($response);
```
For More details visit [intercom reference](https://developers.intercom.io/reference) 
