# Introduction

This is the MediaCT coding standard for Magento 1 projects. It is a mix of the
default MediaCT coding standard and the Magento marketplace standard.

Some tests have been removed from both of the standards to create a workable
and fast standard.

# Installation

Use composer to require the standard in a project.

```shell
$ composer require --dev mediact/coding-standard-magento1
```

To let PHPCS know that this standard should be used add a phpcs.xml file in the
root of the project.

```xml
<?xml version="1.0"?>
<ruleset>
    <rule ref="./vendor/mediact/coding-standard-magento1/src/MediactMagento1"/>
</ruleset>
```

# Integration with PHPStorm

When the phpcs.xml file exists it will be automatically configured by
`media/coding-standard-phpstorm`. This is triggered by the composer command.

```shell
$ composer install
```

# Contribution guidelines

Contributions are welcome. Please create pull requests which add or remove
tests.