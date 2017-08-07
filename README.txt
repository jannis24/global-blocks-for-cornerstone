=== Global Blocks for Cornerstone ===
Contributors: michaelbourne, royanger
Donate link: https://xthemetips.com
Tags: cornerstone, global blocks, x theme, themeco, x pro
Requires at least: 4.5
Tested up to: 4.7.4
Stable tag: 1.2.4
License: GPLv3 or later
License URI: https://www.gnu.org/licenses/gpl-3.0.en.html

Adds a global 'content block' element to both Cornerstone and X Pro page builders. 

== Description ==

Global Blocks for Cornerstone adds a global content block functionality to the Cornerstone and X Pro page builders.
Using a CPT, you will be able to create any content you want in Cornerstone, save it, and use the Global Block custom element to add that content block to any post or page.

= Plugin Features =
 
*   Create a content block once and reuse it on multiple pages.
*   Edit that block in one location and the changed will be reflected site-wide.
*   Use either Cornerstone or the basic editor to create your content in the custom post type.
*   Use any shortcodes you desire, all content will be filtered properly before output.
*   Supports Cornerstone custom CSS and JS in the Global Block.
*	Built in shortcode for using the Global Block outside of Cornerstone via [global_block block="123"] where 123 is the ID of the global block template you want to use

Please note, this plugin requires the Cornerstone Page Builder (or X Pro) to be installed and active. [Cornerstone on CodeCanyon](https://codecanyon.net/item/cornerstone-the-wordpress-page-builder/15518868)

== Installation ==

1.  Upload your plugin folder to the '/wp-content/plugins' directory.
2.  Activate the plugin through the 'Plugins' menu in WordPress.
3.  If you recieve a 404 error while editing a block, simply resave your permalinks.

== Frequently Asked Questions ==

= Can I use the basic Wordpress editor instead of Cornerstone on the Global Block CPT? =

Yes, you can add anything that you want. The content will be filtered with 'the_content' prior to being displayed with the custom element.

= What if I place custom CSS in the Cornerstone customizer on my GLobal Block, will it still work on pages where the block is placed? =

Yes, all custom CSS and JS used in the block will be outputted (inline) with the custom block via the custom element in cornerstone.

= Can I make a Global Block with ACF shortcodes and apply that block as a page template for a CPT? =

Yes, you can. There are two ways to do this, the manual way of using editor supports on the CPT, editing the page in Cornerstone and placing the element on the page, or creating a cpt template in PHP that looks for the value of a dynamic select element, and grabs that blocks content. There will be an in-depth tutorial on this shortly.

== Plugin Removal ==

This plugin will delete all Global Blocks that you have created upon uninstallation. If you would like to keep them, simply deactivate the plugin instead.

== Screenshots ==

None yet

== Changelog ==

= 1.2.4 =
* Upgraded licence to GPL3
* Refactored dependency class and theme detection
* For X5 and X Pro: Removed headers and footers from view while editing Global Blocks

= 1.2.3 = 
* Slight edit for theme detection, not critical if it's already working for you.

= 1.2.1 =
* Error fix, important!

= 1.2.0 =
* Compatibility with X Theme v5 and X Pro

= 1.1.3 =
* Fixed error when attempting to use empty shortcode
* Added helper meta box to CPT screen with shortcode for current post

= 1.1.2 =
* Added shortcode for basic editor Global Block placement via [global_block block="123"] where 123 is the ID of the global block template you want to use
* Fixed uninstall procedures
* Fixed custom css and js error when using an old version of Cornerstone

= 1.1.0 =
* Restructured code and added an uninstall.php file

= 1.0.2 =
* Fixed a PHP error when using this plugin without X Theme

= 1.0.1 =
* Add a soft permalink flush on global block save to prevent 404s on some applications

= 1.0.0 =
* Initial Public Version


== Upgrade Notice ==

= 1.2.3 =
If you are having troubles activating this on X Pro, upgrade.

= 1.2.1 =
Mandatory upgrade. Fixes header issues with other plugins.

= 1.2.0 =
Updated for initial release of X5 and X Pro. Upgrade G.B. and resave your permalinks.

= 1.1.3 =
Fixed error when using empty shortcode, added helper meta box to CPT screen.

= 1.1.2 =
Dropped the_content filter support as it was interfering with plugins that add content to every post. Fixed uninstall procedures.

= 1.1.0 =
Codebase was changed to account for different levels of Cornerstone being active or deactivated. Plugin will now delete all global blocks that have been created if the plugin is deleted by the user. This will help keep your database free of clutter.

= 1.0.2 =
Upgrade for users not using X Theme, fixes a PHP error.

= 1.0.1 =
Fixed a rare issue that could cause users to get a 404 error when editing blocks. 

= 1.0.0 =
You can't upgrade, but you can install.