# ionic_fb_integration
Sample ionic (http://ionicframework.com/) app with FB integration. Works both on localhost in browser and on iOS device.

This app is based on tutorial provided at https://ccoenraets.github.io/ionic-tutorial/ionic-facebook-integration.html. However, I did not manage to build a working FB integrated app basing on the ionic tutorial. 

Differences between this project and ionic tutorial are:
* No OpenFB
* Using https://github.com/Wizcorp/phonegap-facebook-plugin plugin. facebookConnectPlugin.js was changed on line 12 
(put 'if (!window.cordova || cordova.platformId == "browser")' 
instead of original 
'if (cordova.platformId == "browser")')
* index.html has an additional element '<div id="fb-root"></div>'

You should provide you FB app's id in file /www/js/_btGlobals.js at line 15 (btGlobals.fbAppId)
