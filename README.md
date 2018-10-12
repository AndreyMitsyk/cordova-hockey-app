# cordova-hockey-app

### Configuration
To use this app, add appId of your Hockey application here:

`www/js/index.js:31`
```
...
onDeviceReady: function() {
   console.log("Device Ready!");
   hockeyapp.start(null, null, "<appid>");
...
```

### How to build and run app

```
cordova build ios --buildFlag='-UseModernBuildSystem=0'
cordova run ios
```
