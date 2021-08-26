# Cordova Android 10 Bug Demonstration

This was created as follows: ```
cordova create cordova-bug 
cd cordova-bug 
cordova plugin rm cordova-plugin-whitelist
cordova platform add android@10.1.0
cordova plguin add cordova-plugin-device
# add hostname to config.xml
cordova run android
```
