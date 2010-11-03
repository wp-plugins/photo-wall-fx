=== Photo Wall FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, photo, wall, image, text, as3, xml, effects, animation, vertical, horizontal, html, css, drag, bar
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

One of the most advanced Photo Walls on the web. Completely XML customizable, without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without any Flash knowledge. You can specify the width and height of the application, the text is HTML/CSS formatted, the skin of the drag bar is customizable. There are multiple roll over/out effects, various options for image expanding along with many background and shade properties. The position can be vertical or horizontal and there are also different properties for images. Other features are present in the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/photo-wall-fx.zip "Photo Wall FX Plugin") (that you have to install and activate) & [Free package](http://www.flashxml.net/free/download/photo-wall.zip "Photo Wall FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **photo-wall-fx** and copy the content of the **free package** there
3. If you copied the **free package** to a location different than the one above, go to **Photo Wall FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[photo-wall-fx][/photo-wall-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Photo Wall FX part of your theme, edit the template files and add `<?php photowallfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Photo Wall FX](http://www.flashxml.net/photo-wall.html "Photo Wall FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/photo-wall-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/photo-wall-fx/images/` and update the `wp-content/flashxml/photo-wall-fx/images.xml` file accordingly

= Additional settings file =

To embed the Photo Wall FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[photo-wall-fx settings="settings2.xml"][/photo-wall-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `photowallfx_echo_embed_code()` function call (for example `<?php photowallfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[photo-wall-fx]` and `[/photo-wall-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `photowallfx_echo_embed_code()` function call (for example `<?php photowallfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[photo-wall-fx width="600" height="300"][/photo-wall-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `photowallfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/photo-wall.html "Photo Wall FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/photo-wall-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/photo-wall.html "Photo Wall FX") is the utility that helps easily customize your Photo Wall FX to fit all your needs.