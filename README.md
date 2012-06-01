# Riloadr for WordPress
Riloadr for WordPress is a cross-browser responsive images loader for WordPress 3.0.0 and up.

A cross-browser jQuery responsive images loader for WordPress: The goal of this library is to deliver optimized, 
contextual image sizes in responsive layouts that utilize dramatically different image sizes at different resolutions 
in order to improve page load time.

This modification is optimized for use with image sizes defined by WordPress via `add_image_size()`.

**Table of Contents**  

1.  [Features](#features)
2.  [How to use](#howto)
3.  [Compatability](#compatability)
4.  [Changelog](#changelog)
5.  [License](#license)

<a name="features"></a>
## 1. Features

* **jQuery Optimized**: Uses WordPress' built-in jQuery to integrate with Riloadr.
* **Easy to configure**: Optimize your templates and include the required files and you're done.
* **Limit application**: The technique will only be applied to images with the class *riloadr*
* **Solid foundation**: The plugin is built with [scribu/wp-scb-framework](https://github.com/scribu/wp-scb-framework)
* **Mirrors the original**: The rest of the features are equivalent to the ones at [tubalmartin/riloadr](https://github.com/tubalmartin/riloadr)

<a name="howto"></a>
## 2. How to use

1. Upload the `riloadr-for-wordpress` folder to your plugins directory (ie. `/wp-content/plugins/`)
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Set options from the Settings->Riloadr menu
4. Make sure your stylesheet is set up with the following CSS:
	<code><pre>img {max-width: 100%;}
	.lt-ie8 img{-ms-interpolation-mode: bicubic;}
	.lt-ie7 img{width: 100%;}</pre></code>

<a name="compatability"></a>
## 3. Compatability

This technique is tested to work with WordPress 3.3.2+, but should theoretically be backwards compatible to 3.0.

As per [tubalmartin/riloadr](https://github.com/tubalmartin/riloadr) the following browsers have been tested:

**Mobile browsers**

* Webkit mobile (iOS and Android)
* Opera Mini (iOS and Android). Yes, it sounds incredible!!
* Opera Mobile (iOS and Android)
* Firefox mobile (Android)
* Netfront Life browser v2 (Android)
* Dolphin Browser HD (iOS and Android)
* UC Browser 8+ (Android)

**Desktop browsers**

* Internet Explorer 6+
* Firefox (Mac and Win)
* Google Chrome (Mac and Win)
* Safari (Mac and Win)
* Opera (Mac and Win)

<a name="changelog"></a>
## 4. Changelog

Mirrors the [changelog at WordPress.org](http://wordpress.org/extend/plugins/riloadr-for-wordpress/changelog/). Uses [Semantic Versioning](http://semver.org/).

### 1.2.0
* Plugin is now considered stable.
* Core script updated to Riloadr version 1.2.0.
* Script is now minified by default, see [GitHub/OleVik/riloadr-wordpress](https://github.com/OleVik/riloadr-wordpress) for uncompressed script.
* Introduces the experimental **ignoreLowBandwidth** feature.
* Bugfix for the *belowFold* option.

### 1.1.2
###### Bug Fix Release:
* Core script updated to Riloadr version 1.1.0.
* Simplified sizing method.
* Horizontal and Vertical images should now both have Riloadr applied, **irrespective of captions**.

### 1.1.1
###### Bug Fix Release:
* Riloadr is now applied to images outside of captions.
* Horizontal and Vertical images should now both have Riloadr applied.
* Added fallback to original size image, when all else fails.

### 1.1.0
* Public Beta

### 1.0.0
* Private Beta

### Pre 1.0.0
* Private Development

<a name="license"></a>
## 5. License

Copyright (c) 2012 Tubal Martin, Ole Vik

Riloadr for Wordpress is licensed under the [MIT license](https://github.com/OleVik/riloadr-wordpress/blob/master/LICENSE.txt), the plugin itself is licensed as [GPLv2](https://github.com/OleVik/riloadr-wordpress/blob/master/riloadr-for-wordpress/LICENSE.txt).