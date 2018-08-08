MFileChooser (Evolution36 version)
============

Cordova/Phonegap plugin that supplies a File Chooser for Android 4+. The File Chooser does not require installation external file manager.

![alt text](http://i1204.photobucket.com/albums/bb408/krestor85/71df8523-0e50-48d0-a397-b00498910293_zpsd97df182.png "Screenshot 1") | ![alt text](http://i1204.photobucket.com/albums/bb408/krestor85/d11eda8a-8c37-4d9c-8890-eb96cfd07977_zpsdd9f0bf3.png "Screenshot 2")

## Adding the Plugin to your project ##

Plugin has been successfully tested on Android 4+ device with Cordova 5.

To install the plugin

```
cordova plugin add cordova-plugin-mfilechooser
```

## Using the plugin ##

The plugin creates the object `window.plugins.mfilechooser`. To use, call the `open()` method:

### Simple using ###

```javascript
   window.plugins.mfilechooser.open([], function (uri) {
      
      alert(uri);
      
    }, function (error) {
      
        alert(error);
    
    });
```

### Filtering by extension ###

```javascript
   window.plugins.mfilechooser.open(['.doc', '.xls', '.ppt'], function (uri) {
      
      alert(uri);
      
    }, function (error) {
      
        alert(error);
    
    });
```

## Release notes ##

1.0.5: Fix res paths for Cordova 7 and updated README and package id

1.0.4: Fix support dependency and change package name to cordova standards

1.0.2: August 14, 2015 Initial release

## Contribution ##

This plugin is exactly the same as [Maginsoft FileChooser](https://github.com/MaginSoft/MFileChooser) all that we added is the option for the application to rotate with the device's rotation. 
