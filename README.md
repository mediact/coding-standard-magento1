# [ABANDONED] Introduction

This is the MediaCT coding standard for Magento 1 projects. It is based on 
the default MediaCT coding standard but some tests have been removed to create
a workable and fast standard.

# Installation

Use composer to require the standard in a project.

```shell
composer require --dev mediact/coding-standard-magento1
```

To let PHPCS know that this standard should be used add a phpcs.xml file in the
root of the project.

```xml
<?xml version="1.0"?>
<ruleset>
    <rule ref="./vendor/mediact/coding-standard-magento1/src/MediactMagento1"/>
</ruleset>
```

# Integration with PHPStorm and automatic testing

The recommended way to enable the coding standard in PHPStorm and automatic
testing is by requiring the MediaCT testing suite in a project.

```shell
composer require --dev mediact/testing-suite
```

For more information go to [MediaCT Testing Suite](https://github.com/mediact/testing-suite).

# Contribution guidelines

Contributions are welcome. Please create pull requests which add or remove
tests.
