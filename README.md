## MetaPackage repository for Shopgate's Magento2 extensions

### Usage

Go to magento 2 root folder and add magento metapackage name to the require list, e.g.:
```
composer require shopgate/cart-integration-magento2-m2:2.9.7
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
