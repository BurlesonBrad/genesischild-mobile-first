#GenesisChild Mobile First

This theme is a **Mobile First** version of GenesisChild - https://github.com/neilgee/genesischild

This is a basic starter **Genesis Child Theme** to be used with the **Genesis Framework** on **WordPress**.

This Genesischild theme has a number of widgets areas, the majority are Front Page only.

###Widgetised Areas
- The theme contains the following widgetized areas
* Pre-Header Left
* Pre-Header Right
* Header Right
* Hero - Home Page only *front-page.php*
* Optin - Home Page only *front-page.php*
* Home Top - Home Page only *front-page.php*
* Home Middle - Home Page only *front-page.php*
* Home Bottom - Home Page only *front-page.php*
* Before Content *posts only*
* After Content *posts only*
* Footer Widget Header
* Footer Widgets 1, 2, 3
* Footer
* Post Footer Left
* Post Footer Right

###Home Page
The Home Page has been widgetized and the default Genesis loop can be removed.


To remove the Genesis home page loop tweak the **front-page.php** file by uncommenting line 88:
```php
gc_genesis_no_content();
```

and commenting line 90:
```php
//genesis();
```

###Example
For an online visual:
http://themes.wpbeaches.com/genesischild-mobile-first/
Widget areas have background color and content applied to show boundaries.

###Menus
- Primary Menu is positioned above Header Right Widget Hook and is set to Primary Location
- Secondary Menu remains in default area and is Secondary Location spanning full width below the logo/header right.
- Responsive menu is added but not enabled, to enable it uncomment in *functions.php* line 39 *	// include_once( get_stylesheet_directory() . '/includes/responsive-menu.php' );*

###Custom Logo
- Custom Logo is supported via the Customizer, suggested size is 400x150px which you can change in the *add_theme_support('custom-logo')* array in *functions.php*
- The header logo  uses an `<img>` element and can support the SVG format.

###Background Image
- Background Images is supported, a background image can be uploaded in the WP Dashboard via Appearance > Background, this will scale to fit any viewport via BackStretchJS.

To use this you have to enable the BackStretch script in */includes/scripts-styles.php* at line 54

###Customizer
- Customizer options, you can set colors for the options below...
  - link,
  - link hover
  - menu,
  - menu hover,
  - button,
  - button hover,
  - footer links,
  - footer links hover,
  - footer widgets background color

- Site Identity > Logo upload
- Featured Images > background image behind Hero Widget

###Featured Custom Post Type Widget for Genesis
- Bundled in the theme is the 'Featured Custom Post Type Widget for Genesis', the widget is available from the normal widget area in the dashboard *Appearance > Widgets*.

This widget builds on the default Genesis supplied Featured Post widget but can also display Custom Post Types and Taxonomies as well as output them in columns.

*Ref - https://github.com/calliaweb/featured-custom-post-type-widget-for-genesis


###Javascripts
All scripts are in */includes/scripts-styles.php*
- FontAwesome is enabled.
- backstretch.min.js is enabled (via CDN) if a custom background is used. (disabled)
- FItVids is disabled

###CSS
- Regular style.css with all Genesis Framework and placeholders to start new project
- 1 x IE styles in CSS directory for IE9 and lower

###Media Queries
- 2 x CSS min breakpoints are used: min 768px which covers iPad + desktop layout and then wider screens at min 1200px.

###WooCommerce
- WooCommerce style sheet set to load before main style sheet
- Some generic CSS styles declared in styles.css
- WooCommerce theme support declared as an action in *woocommerce.php* but commented out - the *woocommerce.php* file is on *includes* and is called in via *functions.php* as an include, this is commented out be default.
- Use Genesis Connect for WooCommerce plugin - https://wordpress.org/plugins/genesis-connect-woocommerce/

###Miscellaneous
- PHP is enabled to execute in widget areas
- Shortcode enabled in widget areas
- 'Read More' link is enabled on post excerpts
- HTML Tags and Attributes is removed from comments
- The font 'Open Sans' is enqueued from Google Fonts in *includes/scripts-styles.php*
- Author name removed in Post Meta for posts
- SVG support for image uploads
- Beaver Builder full width CSS styles added - leaves header and footer elements intact but full width for inner page.
- Genesis Theme defaults now in */includes*
- Generic landing page added

###Modular Approach
At the top of functions.php there a number of include files that you can comment/uncomment for adding functionality.
- *customize.php* contains all the Customizer options.
- *output.php* renders the Customizer options CSS
- *responsive-menu.php* adds the Genesis Responsive Menu
- *scripts-styles.php* contains all JS and CSS files for inclusion
- *theme-defaults.php* contains all the theme defaults
- *widgets.php* contains all the widgets that need to be registered
- *woocommerce.php* contains all the woocommerce functionality, commented out snippets included
- *class-featured-custom-post-type-widget.php* widget for the Genesis Featured Custom posts

Download the zip rename the theme '**genesischild-mobile-first**' - place this theme in your WordPress installation **"/wp-content/themes/"** and activate in WordPress Dashboard

![Genesis Child Theme](http://wpbeaches.com/images/gcmf-screen.png)

![Genesis Child Theme Customizer](https://wpbeaches.com/images/gc-customizer.png)

![Genesis Child Theme Widget Areas](https://wpbeaches.com/images/gc-screen-widgets.png)
