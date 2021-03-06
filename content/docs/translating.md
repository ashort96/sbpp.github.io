+++
title = "Translating"
description = "Translating Web Panel & Plugin"
date = 2018-02-23T11:58:42-05:00
weight = 24
draft = false
bref = "Fundamental of translating web panel & plugin"
toc = true
+++

### Web Panel

1.  Navigate to the root directory of your SourceBans++ installation's `themes` folder

2.  Make a copy of the `default` theme, rename it to a name of your choosing and navigate to it

3.  Modify `theme.conf.php` to reflect the configuration and save

        <?php
        // Set the name of this theme here
        define('theme_name', "SourceBans++ Default Theme");

        // Set the author of this theme here
        define('theme_author', "IceMan, SourceBans++ Dev Team");

        // Set the version of the theme here
        define('theme_version', "1.5.5-dev");

        // Set the link of the theme here
        define('theme_link', "https://sbpp.sarabveer.me/");

        // Set the screenshot filename for your theme (must be inside your theme folder)
        // Must be:  250px wide  X 170px High
        define('theme_screenshot', "screenshot.jpg");
        ?>

4.  Modify <mark>each</mark> file ending `.tpl` file

5.  Modify the body content of the file

### Plugin

1.  Navigate to SourceMod's `translations` directory

2.  The files you will need to modify are <samp>sourcebans.phrases.txt</samp>, <samp>sourcecomms.phrases.txt</samp>, and <samp>sourcesleuth.phrases.txt</samp>

3.  Within `Phrases` key section, for each sub key sections, append a key value pair, with the two letter language code being the key and the value being the translation (If `#format` kv pair is present, be sure to follow it)

For more information regarding SourceMod translation, view SourceMod's [Translation](<https://wiki.alliedmods.net/Translations_(SourceMod_Scripting)>) article
