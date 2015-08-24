# Notifie JS
Javascript library for displaying notifications

#Instructions for adding to bundle
1. Add CSS and JS file to /<YOUR_THEME_NAME>/libraries/jquery.notifie/ (You will have to create the jquery.notifie directory.)
2. Open head.jspf (Found in /<YOUR_THEME_NAME>/common/interface/fragments/)
3. Import CSS file at the top of head.jspf with the other CSS files
    &lt;link rel="stylesheet" type="text/css" href="&lt;%=bundle.bundlePath()%&gt;libraries/jquery.notifie/jquery.notifie.css" /&gt;
4. Import JS file at the bottom of head.jspf with the other JS files
    &lt;script type="text/javascript" src="&lt;%=bundle.bundlePath()%&gt;libraries/jquery.notifie/jquery.notifie.js"&gt;&lt;/script&gt;

#How to use
Call .notifie(options) on a jQuery element, where options is a Javascript object with settings for the notifications.

Example: 
$('input').notifie({
  type: 'alert',
  severity: 'info',
  message: 'This is an informative notification.'
});

See the JS file for details on what options are available.