=== TIVWP-DM Development Manager ===
Contributors: tivnet
Tags: debug, debugging, development, developer, plugins
Requires at least: 3.8
Tested up to: 3.9-beta1
Stable tag: trunk
License: GPLv2 or later

Install and manage development plugins

== Description ==

TIVWP-DM Development Manager is a plugin for WordPress developers. Its main features are:

* Prompts to automatically install and activate popular development plugins from the WordPress repository
* Allows to activate / deactivate those plugins in bulk - with a single admin menu click or automatically, according to the wp-config settings

For complete information, please see [TIVWP-DM Development Manager's GitHub repo](https://github.com/tivnet/tivwp-dm).

= 3rd Party Software Used =

[TGM-Plugin-Activation](https://github.com/thomasgriffin/TGM-Plugin-Activation) by

* Thomas Griffin <thomas@thomasgriffinmedia.com> and
* Gary Jones <gamajo@gamajo.com>

== Installation ==

You can install this plugin directly from your WordPress dashboard:

1. Go to the *Plugins* menu and click *Add New*.
2. Search for *TIVWP Development Manager*.
3. Click *Install Now* next to the TIVWP Development Manager plugin.
4. Activate the plugin.

Alternatively, see the guide to [Manually Installing Plugins](http://codex.wordpress.org/Managing_Plugins#Manual_Plugin_Installation).

== Frequently Asked Questions ==

= Can I use this plugin on a WordPress Multisite? =

Yes, but you should activate the plugin on each site separately. Network Activation is disabled by default.
To enable, place
`define( 'TIVWP_DM_NETWORK_ACTIVATION_ALLOWED', true );`
in the wp-config.php file.

== Screenshots ==

1. Prompt to install the plugins
2. Use admin menu to (de)activate all development plugins
3. Automatic deactivation with the presence of `define( 'TIVWP_DM_AUTO', 'deactivate' );`

== Changelog ==

= 14.03.19 =
* Better validation of capabilities
* Multisite activation is allowed
* Network Activation is disabled by default

= 14.03.17 =
* Initial release
