# Easy-Columns-PHP-8-Update
An update for the outdated Easy Columns WordPress plugin for PHP 8.

[Easy Columns](https://wordpress.org/plugins/easy-columns/) is an old plugin that hasn't been updated in 10 years. However, many old sites use it, and updating to PHP 8.0 breaks it. 

Previously, the plugin utilized a constructor method named EasyColumns(), which is deprecated in PHP 7 and removed in PHP 8. This deprecated method has been replaced with the standard __construct() method, aligning with PHP 8's requirements. This change allows the plugin to function correctly in environments running PHP 8.

The change was made in line 35 of `easy-columns.php`. Originally it was:

`function EasyColumns() { //constructor`

Updated is: 

`function __construct() { //constructor`

