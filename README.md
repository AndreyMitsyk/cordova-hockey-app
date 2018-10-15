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

1) Install packages and initialize platform:
```
npm install
cordova platform add ios
```

2) Open `platforms/ios/cordova-hockey-app.xcworkspace` in Xcode and select provisioning profile for project and set target.

3) Build and run project
```
cordova build ios --buildFlag='-UseModernBuildSystem=0'
cordova run ios
```

*Note:* You cau update cordova sdk manually: replace content of `plugins/cordova-plugin-hockeyapp` folder.

![cordova-hockey-app](https://github.com/AndreyMitsyk/cordova-hockey-app/raw/master/Image_0.jpg)
