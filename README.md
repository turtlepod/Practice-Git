# Genbu WordPress Theme

## About

**Author:** David Chandra Purnama <br/>
( [@turtlepod](http://twitter.com/turtlepod) / [shellcreeper.com](http://shellcreeper.com/) )

Genbu theme is an clean and simple responsive theme built with search-engine optimization (SEO) in mind by utilizing the most current HTML5 conventions and [Schema.org](http://schema.org) microdata.

More info: [Theme Page](http://genbutheme.com/)

## Features

* (9) Layouts
* (2) Sidebar
* (2) Menus 
* Custom Background
* Custom Header Image
* Editor Style
* Translation Ready

### Layouts
* Content (No Sidebar)
* Content / Sidebar 1
* Sidebar 1 / Content
* Sidebar 2 / Content
* Content / Sidebar 2
* Sidebar 2 / Content / Sidebar 1 (Default)
* Sidebar 2 / Sidebar 1 / Content
* Content / Sidebar 1 / Sidebar 2
* Sidebar 1 / Content / Sidebar 2

Layout info:
* **Content**: Main content of the page.
* **Sidebar 1**: 300px width.
* **Sidebar 2**: 160px width.

### Menus
* **Navigation**<br/>
Located below header with search form on the right side. On mobile device will use toggle and using menu name as toggle. When not set, it will display link to home page.
* **Footer Links**<br/>
Will be displayed as simple links in footer area. If not set, will not be displayed.

### Custom Background:

You can set custom background via WP Customize or Background settings page.

### Custom Header Image:

Genbu have custom header feature you can set custom header image via WP Customize or header settings page.
* **As banner image**: when displaying the header text, the header image will be used as banner image below site title and description.
* **As logo**: when not using header text, header image will be used as logo.

### Editor Style:

Genbu is using editor style, so you'll see what you get in your WordPress visual editor.

### Translation Ready:

You can translate this theme using pot file located at languages folder.

## CSS and JS

### Stylesheets
CSS files loaded in this theme (in order):
* **Open Sans**<br/>
Main font used in this theme.<br/>
Handle: `theme-open-sans-font`<br/>
Style: 400,300,300italic,400italic,600,600italic,700,700italic,800,800italic<br/>
Location: Google Font
* **Dashicons**<br/>
Font icon used in this theme.<br/>
Handle: `dashicons`<br/>
Location: WordPress.
* **Main Stylesheet**<br/>
The main stylesheet.<br/>
Handle: `style` or `parent` (if using child theme)<br/>
Location: style.min.css<br/>
size: 35kb

#### Main Stylesheet:
The Main style.css is a merge and minification of (in order):
* **Reset CSS**<br/>
Base style and set style defaults.<br/>
Handle: `theme-reset`<br/>
Location: css/reset.min.css<br/>
Size: 10kb
* **Menus CSS**<br/>
Base navigation style<br/>
Handle: `theme-menus`<br/>
Location: css/menus.min.css<br/>
Size: 5kb
* **Theme CSS**<br/>
Theme custom style<br/>
Handle: `theme`<br/>
Location: css/theme.min.css<br/>
Size: 16kb
* **Media Queries CSS**<br/>
Responsive style<br/>
Handle: `media-queries`<br/>
Location: css/media-queries.min.css<br/>
Size: 5kb

### JS files used in this theme:
* jQuery (required library): part of WordPress
* Fitvids (responsive video library): js/fitvids.min.js (only 3kb)
* Theme JS (custom and setting for other script): located at /js/theme.min.js (only 2kb)

### Editor CSS files used in this theme (in order):
* Open Sans: via Google Font
* Theme Reset (set default for element styling): located at /css/reset.min.css (10kb)
* Editor Style (if using child theme, child theme /css/editor.css will also loaded): located at /css/editor.css (1kb)

### CSS and JS Override
Child theme can override parent theme CSS and JS by creating the file(s) in the same location except for main stylesheet, parent theme style{.min}.css, external script such as Google Font, and scripts bundled in WordPress such as Dashicons.

### Links

* [Github project page](https://github.com/turtlepod/genbu)
* [Theme page](http://genbutheme.com/)
* Need a custom theme or plugin for your WordPress website? [I can help](http://shellcreeper.com/services/).

## Copyright & license

This theme is licensed under the [GNU General Public License](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html), version 2 (GPL) or later.

2014 © [Genbu Media](http://genbu.me/). All rights reserved.

## Changelog:

### 1.3.0
* update to Hybrid Core version 2.0.3
* update Tamatebako to version 2.0.0
* remove unused scripts and style. child theme should add it themselves (for version compatibility). sorry for this :(
* Editor Style now using minified stylesheet.
* Add [simple jQuery mobile browser detection](http://shellcreeper.com/simple-mobile-browser-detection-using-javascript/).
* CSS is merged to main stylesheet.
* Removing Grunt, make it clean.

### 1.2.2
* use tamatebako_theme_file() and not hybrid_locate_theme_file().
* change hook "genbu_after_theme_setup" to "genbu_after_setup_theme".
* Clean up content folder, add singular template for all post format.
* Fix content error notice (404 pages).
* Add skip to content in plugins template files.
* Quick fix of sub menu toggle.
* Now using GIT and no longer SVN
* Fix Tamatebako, see includes/tamatebako-changelog.md for detail.
* Update Hybrid Core to version 2.0.2
* Remove wp_link_pages args in content/*.
* Remove all blank index.html

### 1.2.1
* Update minified.

### 1.2.0
* Use Grunt (private use): node_modules folder, package.json, and Gruntfile.js is not added in theme.
* Change stylesheet load method.
* add editor-style.css (reset.css + style.css)
* and theme.css (all css loaded in theme into one minified css)
* use POT file for translation, remove po and mo file.
* Fix mbile Sub-Menu Toggle (jQuery)
* Fix Pre element display (overflow) on mobile.
* Fix Editor Style (WP 4.0 Editor Auto resize feature).

### 1.1.0
* add license.txt
* update tamatebako to version 1.0.1
* fix media queries menu, and add dash 1st sub-menu too.
* update translation file.
* add class ".comments-section" to "#comments-template" in "comments.php"
* Update HC to version 2.0.1 + Tamatebako 1.1.0
* Update lang files

### 1.0.0
* Push to version 1.0.0
* now using [Semantic Versioning](http://semver.org/)

### 0.1.4
* Disable comment error on Page (post type).
* Add basic support for WooCommerce Plugin.
* Add basic support for The Events Calendar Plugin.
* Add basic support for Easy Digital Downloads Plugin.
* Add basic support for Custom Content Portfolio Plugin.
* Fix search form (menu) toggle, now using link instead of button.
* Remove Utility functions from template, add examples in docs folder.
* Change global for widget num to tamatebako.
* Fix tag footer to div in entry footer for plural pages.
* Change header tag to div in comment meta.
* Fix threaded comments style
* Add basic support and style for Post Formats.
* Add thumbnail for post archive.
* Better layout structure to enable grid/columns in displaying posts list.
* Add base structure and example for grid and masonry in displaying posts list.
* Add flexslider and examples in how to use it.
* Restructure "tamatebako"; better inline docs; remove "edit *" filter.

### 0.1.3
* Read more no longer using filter, now using template function.
* Better Accessibility Feature for Menus and Links
* bbPress and BuddyPress Support
* Update translation
* Better Default WP Title
* Update styling for readibility
* Separate load for reset(base) CSS and Menus CSS
* Fix Editor Style

### 0.1.2
* Better style
* Better read more

### 0.1.1
* Fix string function
* Fix css bug
* Add custom header image support

### 0.1.0
* Initial version
