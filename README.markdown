Redirect app install script for WebFaction
==========================================

[Click here to install](https://my.webfaction.com/app/create?script_url=https://raw.github.com/wsfulmer/webfaction-redirect-installer/master/install)

This creates a static app with a .htaccess file that does a redirect to the URL
that you specify in the 'extra info' field.

The generated .htaccess will look like this:

    Options +FollowSymLinks
    RewriteEngine on
    RewriteRule ^(.*)$ http://destination.com/$1 [R=301,L]

Add this app to a site that uses the domains that you want to redirect to the
destination domain.

The app cannot be modified in the control panel after it has been created. If
you need to change the redirect, then edit the .htacess file directly, or
delete this redirect app and create a new one.


