PhoneGap\XDK Cordova plug-in for Yandex Metrica 2.0

Android and iOS are supported

Three methods supported:

window.AppMetrica.activate('key here', [ success, fail]);

window.AppMetrica.reportEvent('event' ,[ success, fail]);

window.AppMetrica.reportEventJson('event', json ,[ success, fail]);

<b>Instalation<b>
Install CocoaPods

<code>cd to iOS platform folder<br>
run pod install

in app.js add <br>
$ionicPlatform.ready(function() {<br>
window.AppMetrica.activate('key here', [ success, fail]);<br>
...
}
</code>
