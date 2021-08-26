# Cordova Android 10 Bug Demonstration

This was created as follows: 

```
sudo npm install -g cordova
cordova create cordova-bug 
cd cordova-bug 
cordova plugin rm cordova-plugin-whitelist
cordova platform add android@10.1.0
cordova plugin add cordova-plugin-device
# add hostname to config.xml
cordova run android
```

Alternatively, you could run this Cordova project:
```
sudo npm install -g cordova
git clone https://github.com/codeconsole/cordova-bug
cd cordova-bug
cordova prepare
cordova run android
```
