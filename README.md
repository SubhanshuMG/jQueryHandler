# jQuery error capturing plugin

This jQuery plugin send an email when a javascript error is triggered. 
Specially useful in big web application where you want to know if users hit javascript errors.

A php mail example is given with this plugin, but it could also be easily logged in a database 

## Integration

Load the plugin just after the jQuery library

      $(document).jsErrorHandler();



## Options

You can define some options.

By default the plugin automatically fetch the domain and add it to the email subject, but you can overwrite it.
You can also define a from, I would highly recommend that you change the from setting in the plugin file (jquery.onerror.js)  if your going to use this plugin on multiple websites.

     $(document).jsErrorHandler({
        from: "support@youremail.com",
		website: document.domain
     });
