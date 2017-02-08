##PhoneGap Cordova Ionic plug-in for AppMetrica (Yandex) ^2.0##

Android and iOS are supported

Three methods supported:

```javascript
window.AppMetrica.activate('API key', [ success, fail]);

window.AppMetrica.reportEvent('event' ,[ success, fail]);

window.AppMetrica.reportEventJson('event', json ,[ success, fail]);
```
###Instalation###

Install CocoaPods


```
cordova plugin add https://github.com/tetrakiss/AppMetricaCordovaPlugin.git
cordova prepare
cd to iOS platform folder
run pod install
```
register new app https://appmetrica.yandex.ru/application/new <br>
get API KEY

###in app.js add ###

```javascript
$ionicPlatform.ready(function() {
window.AppMetrica.activate('API key', [ success, fail]);
...
}
```

###in controller add ###
```javascript
.controller('MyCtrl', function($window) {
 $window.AppMetrica.reportEventJson('EVENT NAME' , {'key': 'value', 'key': 'value' }, [success, fail]);
...
}

```
