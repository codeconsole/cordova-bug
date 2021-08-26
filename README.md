# cordova-android@10.1.0 Bug Demonstration

The deviceready is not fired on Android when running `cordova-android@10.#.#` with the cordova-plugin-device installed.

This was created as follows: 

```
# Install the latest version of Cordova
sudo npm install -g cordova 
# Create the app
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
# Install the latest version of Cordova
sudo npm install -g cordova # Install the latest version of Cordova
# Chekout the app
git clone https://github.com/codeconsole/cordova-bug
cd cordova-bug
cordova prepare
cordova run android
```

A workaround for fixing the problem is to add the following preference to config.xml
```
<preference name="AndroidInsecureFileModeEnabled" value="true" />
```
