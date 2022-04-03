# WP-Flash & Ruffle Plugin for WordPress
The [WP-Flash & Ruffle plugin](https://www.cyberseo.net/wp-flash/) allows you to easily insert Adobe Flash animation into WordPress blog posts and pages. The plugin supports both [Adobe Flash Player](https://www.adobe.com/products/flashplayer.html) and [Ruffle Flash Player emulator](https://ruffle.rs/).

Use the following shortcode to insert Adobe Flash animation into your posts and pages:

`[swf:url width height bgcolor wmode]`

where:
* __url__: URL of the flash object (SWF file) you want to embed;
* __width__: width of the flash object;
* __height__: height of the flash object;
* __bgcolor__: background color (optional);
* __wmode__: wmode, e.g. transparent (optional).

For more information about the above attributes, see [this Adobe support page](https://helpx.adobe.com/flash/kb/flash-object-embed-tag-attributes.html).

## Summary of Changes
I've made the following changes to the original source:
* Besides its main function, the original version inserted a banner ad. I've removed this "feature."
* Ruffle is now loaded from an [auto-updating CDN](https://unpkg.com/browse/@ruffle-rs/ruffle/). No need to manually update it anymore.
* The plugin now adds a convenient link to its Settings page onto the WordPress Plugins management page.
