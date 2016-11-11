S-Money Bundle
==============

## Get the bundle using composer

Add SmoneyBundle by running this command from the terminal at the root of
your Symfony project:

```bash
composer require smoney/smoney-bundle
```


## Enable the bundle

To start using the bundle, register the bundle in your application's kernel class:

```php
// app/AppKernel.php
class AppKernel extends Kernel
{
    public function registerBundles()
    {
        $bundles = array(
            // ...
            new Smoney\SmoneyBundle\SmoneyBundle(),
            // ...
        );
    }
}
```

## Configure the bundle

```yaml
# app/config/config.yml
    smoney:
        api_token: YOUR_TOKEN
        api_version: v1  #Global version to use for the API (can be override with SetVersion in any service)
        api_base_url: https://rest-pp.s-money.fr/api/sandbox

```
