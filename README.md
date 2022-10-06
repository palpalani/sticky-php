# Sticky Subscription Commerce Platform PHP Client

https://sticky.io/

[![Latest Stable Version](https://poser.pugx.org/palpalani/sticky-php/v/stable?format=flat-square)](https://packagist.org/packages/palpalani/sticky-php)
[![License](https://poser.pugx.org/palpalani/sticky-php/license?format=flat-square)](https://packagist.org/packages/palpalani/sticky-php)

## Installation

To install, use composer:

```
composer require palpalani/sticky-php
```

## Documentation

https://developer-prod.sticky.io/?version=latest

### Example Usage

```php
$limelightCRM = new LimeLightCRM([
    'base_url' => 'your_url',
    'username' => 'your_username',
    'password' => 'your_password'
]);

$limelightCRM->transaction()->newOrder([
    'firstName'  => 'John',
    'lastName' => 'Doe',
    'email' => 'jdoe@gmail.com'
]);

$limelightCRM->transaction()->newOrderWithProspect([
    'firstName'  => 'John',
    'lastName' => 'Doe',
    'email' => 'jdoe@gmail.com'         
]);

$limelightCRM->membership()->findActiveCampaign();

$limelightCRM->membership()->viewCampaign([
    'campaign_id' => 1     
]);

```


## Testing

```bash
composer test
```

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Security Vulnerabilities

Please review [our security policy](../../security/policy) on how to report security vulnerabilities.

## Credits

- [palPalani](https://github.com/palpalani)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
