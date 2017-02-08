##PhoneGap\XDK Cordova plug-in for Yandex Metrica 2.0##

Android and iOS are supported

Three methods supported:

```javascript
window.AppMetrica.activate('key here', [ success, fail]);

window.AppMetrica.reportEvent('event' ,[ success, fail]);

window.AppMetrica.reportEventJson('event', json ,[ success, fail]);
```
###Instalation###

Install CocoaPods

`cd to iOS platform folder
run pod install`

###in app.js add ###

```javascript
$ionicPlatform.ready(function() {
window.AppMetrica.activate('key here', [ success, fail]);
...
}
```
