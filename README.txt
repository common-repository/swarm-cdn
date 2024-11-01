=== Swarmify (legacy image plugin) ===
Version: 0.4.1
Donate link: https://swarmify.com/
Stable tag: trunk
License: GNU AFFERO GENERAL PUBLIC LICENSE
License URI: http://www.gnu.org/licenses/agpl-3.0.html

Allows you to easily configure your WordPress site to use Swarmify.

== Description ==
## Note (Dec. 2018):
> This plugin is for a legacy offering on which no new development is expected. Please use our new [Video Hosting Plugin](https://wordpress.org/plugins/smartvideo/) as it offers the best experience with Swarmify

[Swarmify Video Hosting](https://swarmify.com/) is the first unlimited video cdn.
This WordPress plugin, supports a legacy offering which offloaded image delivery for your website. Please instead use our [newer plugin](https://wordpress.org/plugins/smartvideo/).

No new releases of this plugin are to be expected.


== Installation ==

1. Copy the `swarm-cdn` directory into your `/wp-content/plugins/` directory.
2. Activate the plugin through the *Plugins* menu in your WordPress Dashboard.
3. Navigate to the newly created *Swarmify* menu item, under the *Settings* menu in your WordPress Dashboard.
4. Configure the Swarmify plugin settings.

= Known Issues =

**Lazy Loading** - If you're using a Lazy Loading script go ahead and turn it off as it conflicts with our script and the best part is we already use Lazy Loading.


== Changelog ==
= 0.4.1 =
Change to load script over SSL by default

= 0.4.0 =
Prevented image swarming when the website is being accessed by a bot or other search engine. This is to ensure
proper crawling, indexing and SEO optimizations.

= 0.3.9 continued =
Changed branding from Swarm CDN to Swarmify. Retained version number as this is not a bug fix or functional update.

= 0.3.9 =
Added back in output buffering that was removed in 0.3.4 as an optional feature, defaulted to off.

= 0.3.8 =
Fixed a bug that would sometimes cause the Media Manager to not display any items for "All Media" or "Video" filters when the Swarm CDN plugin was active.

= 0.3.7 =
Added attributes to Swarm script tags to disable Cloudflare's async loading. This was accidentaly removed in version 0.3.4

= 0.3.6 =
Added back in filtering of 'the_content' that was present in 0.3.4, while maintaining the new filtering of 'the_posts' added in 0.3.5

= 0.3.5 =
Fixed a bug introduced by v0.3.4 that was not properly handling swarmed content in all page types.

= 0.3.4 =
Removed output buffering as it appeared to conflict with output buffering in other plugins.

= 0.3.3 =
Added additional embed options when embedding MP4 videos using Swarm CDN.
Moved the "Insert with Swarm CDN" button on the media-manager to a more obvious location.
Hid the default "Insert into Post" button so as not to confuse users on which one to use.
Changed the readme.txt plugin name to match the actual plugin name (Swarm CDN) once it is installed.

= 0.3.2 =
Fixed a permissions issue when writing out swarmcdniframe.html by changing the target directory to "uploads".
Added in a "swarmiframe" variable to the page-injected javascript which indicates the location of swarmcdniframe.html

= 0.3.1 =
Adding in missing jQuery Select2 dependencies.

= 0.3.0 =
Enhanced video support with embeddable SwarmCDN shortcodes. Check the SwarmCDN settings page after installing to get started.

= 0.2.1 =
Fixed a sanitization bug when saving settings that would allow the Swarm code to appear without a proper api key.

= 0.2.0 =
Added multisite support.

= 0.1.8 =
Performance improvements.

= 0.1.7 =
Fixed a pathing bug.

= 0.1.6 =
Added in a version check routine to run logic when the plugin is updated as the activation hook does not run on updates.

= 0.1.5 =
Fixed the 1x1 place holder graphic to use relative protocol.

= 0.1.4 =
Fixed a bug that would clear the plugin settings when the main WordPress settings were updated.

= 0.1.3 =
Modified script tags so that CloudFlare's Rocket Loader will ignore Swarm CDN scripts.
