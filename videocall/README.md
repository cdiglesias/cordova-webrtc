# Video Conferencing / [online demo](https://rtcmulticonnection.herokuapp.com/demos/Video-Conferencing.html) / [install from appstore](https://play.google.com/store/apps/details?id=rmc3.videoconference)

APK files and other source codes can be found here:

* https://webrtcweb.com/cordova-apps/video-conferencing/

# First of All:

```sh
# We must install this version because does work correctly with the last version on iOS
npm -g install cordova@8.0.0
```

```sh
yarn
```

# Deploy on Android Platforms

Path: `./platforms/android/AndroidManifest`

Find `<uses-sdk` and paste following code quickly after that line:

```xml
<uses-sdk android:targetSdkVersion="26" />
<uses-permission android:name="android.permission.CAMERA" />
<uses-permission android:name="android.permission.MICROPHONE" />
<uses-permission android:name="android.permission.MODIFY_AUDIO_SETTINGS" />
<uses-permission android:name="android.permission.RECORD_AUDIO" />
<uses-permission android:name="android.permission.WAKE_LOCK" />
```

```sh
yarn android
```


# Deploy on iOS Platforms
Open xcode and assign Credentials

After that, run this command

```sh
yarn ios
```

---

For more info, please check:

* [docs/ios-android.md](https://github.com/muaz-khan/RTCMultiConnection/blob/master/docs/ios-android.md)

# License

[All Cordova Mobile Apps](https://github.com/muaz-khan/cordova-mobile-apps) are released under [MIT licence](https://www.webrtc-experiment.com/licence/) . Copyright (c) [Muaz Khan](https://plus.google.com/+MuazKhan).
