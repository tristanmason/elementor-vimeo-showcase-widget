# Vimeo Showcase Widget for Elementor

This Wordpress plugin adds a widget to Elementor which accepts a vimeo showcase ID and embeds the showcase. It does not use the Vimeo API; it simply adds the ID to Vimeo's standard showcase embed code and spits that code out on the page. The main purpose of this plugin is to allow embedding of Vimeo showcases in Elementor without using <iframe> tags in an Elementor HTML widget, because those get stripped out in a Wordpress Multisite environment unless the user is a super admin. This widget allows editors and non-super admins to easily embed Vimeo showcases.

## Installation

Download as a ZIP file and upload using the normal Wordpress "Add Plugin" dialog.

## Plugin Structure: 
```
assets/
      /js
      
widgets/
      /embed-vimeo-showcase.php
      
index.php
elementor-embed-vimeo-showcase.php
plugin.php
```

* `assets` directory - Holds plugin JavaScript and CSS assets
  * `/js` directory - Holds plugin JavaScript Files
* `widgets` directory - Holds plugin widgets
  * `/embed-vimeo-showcase.php` - Embed Vimeo Showcase Widget class and Wordpress plugin meta info
* `index.php`	- Prevent direct access to directories
* `elementor-embed-vimeo-showcase.php`	- Main plugin file, used as a loader if plugin minimum requirements are met.
* `plugin.php` - Main plugin class

For more documentation please see [Elementor Developers Resource](https://developers.elementor.com/creating-an-extension-for-elementor/).
