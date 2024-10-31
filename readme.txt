=== Options Optimizer ===
Tags: autoload, options, memory, optimize
Stable tag: 1.0
Donate link: http://www.blogseye.com/buy-the-book/
Requires at least: 3.1
Tested up to: 3.5
Contributors: Keith Graham
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Optimizes options by changing autoload values or deleting orphaned options.

== Description ==
The Options Optimizer allows you to change plugin options so that they don't autoload. It also allows you to delete orphan options.

In WordPress, some options are loaded whenever Wordpress loads a page. These are marked as autoload options. This is done to speed up WordPress and prevent the programs from hitting the database every time some plugin needs to look up an option. Automatic loading of options at start-up makes WordPress fast, but it can also use up memory for options that will seldom or never be used.

You can safely switch options so that they don't load automatically. Probably the worst thing that will happen is that the page will paint a little slower because the option is retrieved separately from other options. The best thing that can happen is there is a lower demand on memory because the unused options are not loaded when WordPress starts loading a page.

When plugins are uninstalled they are supposed to clean up their options. Many options do not do any clean-up during uninstall. It is quite possible that you have many orphan options from plugins that you deleted long ago. These are autoloaded on every page, slowing down your pages and eating up memory. These options can be safely marked so that they will not autoload. If you are sure they are not needed you can delete them.

You can change the autoload settings or delete an option on the form below. Be aware that you can break some plugins by deleting their options. I do not show most of the built-in options used by WordPress. The options list should be just plugin options. 

It is far safer to change the autoload option value to no than deleting an option. Only delete an option if you are sure that it is from an uninstalled plugin.
  
In order to see if the change in autoload makes any difference, you can view the source of your blog pages and look for an html comment that shows your current memory usage and the load time for the page. This is added to the footer by this plugin. This is an HTML comment so you will have to view the page source and look for something like:

Options Optimizer: 
29 queries in 0.282 seconds.
Memory Usage Current: 13,893,944, Peak: 14,272,364
 
Deactivate the plugin when not in use. 

== Installation ==
1. Download the plugin or add plugin directly from the WordPress plugin repository.
2. If you download the plugin you then must upload the plugin to your wp-content/plugins directory.
3. Activate the plugin.
4. The settings page for the plugin will let you change or delete options.

== Changelog ==

= 1.0 =
* initial release 

== Support ==
* This plugin is free and I expect nothing in return. Please rate the plugin at:
* http://wordpress.org/extend/plugins/options-optimizer/
* If you wish to support my programming, buy my book: 
* <a href="http://www.blogseye.com/buy-the-book/">Error Message Eyes: A Programmer's Guide to the Digital Soul</a>
* Other plugins:
* <a href="http://wordpress.org/extend/plugins/permalink-finder/">Permalink Finder Plugin</a>
* <a href="http://wordpress.org/extend/plugins/open-in-new-window-plugin/">Open in New Window Plugin</a>
* <a href="http://wordpress.org/extend/plugins/kindle-this/">Kindle This - publish blog to user's Kindle</a>
* <a href="http://wordpress.org/extend/plugins/stop-spammer-registrations-plugin/">Stop Spammer Registrations Plugin</a>
* <a href="http://wordpress.org/extend/plugins/no-right-click-images-plugin/">No Right Click Images Plugin</a>
* <a href="http://wordpress.org/extend/plugins/collapse-page-and-category-plugin/">Collapse Page and Category Plugin</a>
* <a href="http://wordpress.org/extend/plugins/custom-post-type-list-widget/">Custom Post Type List Widget</a>

