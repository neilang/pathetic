===================
= Pathetic Module =
===================

The pathetic module will alter absolute urls (specified by you) to make sure they are always server relative.

This is handy for drupal developers who use multiple development environments OR sites that have authors who accidentally paste in absolute urls to development/test servers.

You can set an unlimited amount of domains you want to be considered server relative. Pathetic will alter anchor "href" attributes and image "src" attributes.

================
= Installation =
================

1. Place the module in the modules directory and enable it as per usual.

2. Navigate to Administer > Site Configuration > Input formats.

3. Click "configure" on the input format you want to apply this filter too.

4. Under the "filters" group, enable "Pathetic Filter" and save.

5. To specify the domains you would like to consider internal absolute references, click "configure" on the filter then select the "configure" tab.
   
6. In the "Pathetic filter" group there is a textarea "Domains to strip", add your domains there.

Example:

http://www.example.com/
http://example.com/
http://development.example.com/
http://www.example.com:80/
http://localhost/
http://127.0.0.1/
