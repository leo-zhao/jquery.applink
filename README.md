jquery.applink
==============

Create links to native apps from mobile (or minor cases from desktop) browsers.

HTML links should have the web url as default, but you can add an alternate link using the registered app protocol to invoke apps like Facebook, Twitter, Foursquare, etc...

Example:

    <a href="https://facebook.com/me" data-applink="fb://profile">My Facebook Profile</a>

Also, you can use it to share your page, like:

    <a href="http://twitter.com/intent/tweet?url=<?php echo $url; ?>&amp;text=<?php echo urlencode($text); ?>" data-applink="twitter://post?url=<?php echo $url; ?>&amp;text=<?php echo urlencode($text); ?>">Share My Web in Twitter</a>

This action will try to open the Twitter mobile app, and if is not available, it will open the default share modal at browser.

You have a extended schemes list available at http://wiki.akosma.com/IPhone_URL_Schemes

To enable the plugin:

    $('a[data-applink]').applink();

Enjoy!
