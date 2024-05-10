## Meta-Package for Shopgate's Magento 2 Extensions

References the extensions required for a Shopgate Go integration.

### Usage

Go to Magento 2 root folder and require the package via Composer:
```
composer require shopgate/cart-integration-magento2-m2:^2.9.43 --update-with-dependencies
```

This will install all three extensions required for Shopgate to run in the vendors/shopgate folder:

* Shopgate_Base
* Shopgate_Export
* Shopgate_Import

Enable the extensions and upgrade the database schemas:
```
bin/magento module:enable Shopgate_Base Shopgate_Export Shopgate_Import
bin/magento setup:upgrade
```

### Changelog

Changes will be documented in the respective referenced packages, see:
* [Base](https://github.com/shopgate/cart-integration-magento2-base/blob/master/CHANGELOG.md)
* [Export](https://github.com/shopgate/cart-integration-magento2-export/blob/master/CHANGELOG.md)
* [Import](https://github.com/shopgate/cart-integration-magento2-import/blob/master/CHANGELOG.md)
