## UnityAds 2 Plugin 

Cordova / PhoneGap Plugin for UnityAds ver 2.x

## Contents

1.  [Description](#description)
2.  [Plugin Background](#history)
3.  [Features](#features)
4.  [Quick Start](#quick-start)
5.  [Installation](#installation)
6.  [Usage](#usage)
7.  [Methods](#api)
8.  [Screenshots](#screenshots)
9.  [Credits](#credits)
10. [Donations](#donations)

## DESCRIPTION

This Cordova / PhoneGap plugin enables the integration of Unity Ads video ads into your cordova mobile games or apps in a way that both increases player engagement and puts more money in your pocket over the gamer’s lifetime. Unity Ads offers the highest Average Revenue Per User (ARPU) of any global rewarded video ad network.


## PLUGIN BACKGROUND

A couple of years ago, and after a great mistake, I got banned from Google AdsMob network. After appels to the mercy of Google, explaining what happens... I remain banned for life.  This put me on a very bad situation those days, with a very short list of good monetizing alternatives.  This ends the day I learn about UnityAds

After the end of the UnityAds 1.x Api era, I have to move forward and Implement UnityAds 2.x on my projects. Implement it on the Unity Game Engine was a breeze, But then I didn't found any solutions to implement version 2.x on my html5, cordova, construct 2 or 3 projects.  That my friends, makes this cordova plugin a reality. Oh well, it was basically only necessity!

## FEUTURES

Platforms supported:
- [x] iOS, via SDK v2.x.x (see [Release Notes](https://github.com/Unity-Technologies/unity-ads-android))
- [x] Android, via Android SDK v2.x.x (see [Release Notes](https://github.com/Unity-Technologies/unity-ads-ios))

Ad Types:
- [x] Non Rewarded Video
- [x] Rewarded Video


## QUICK START
```bash
	# create a demo project
    cordova create test1 com.rjfun.test1 Test1
    cd test1
    cordova platform add android
    cordova platform add ios

    # now add the plugin, cordova CLI will handle dependency automatically
    cordova plugin add com-artemisoftnian-plugins-unityads2

    # now remove the default www content, copy the demo html file to www
    rm -r www/*;
    cp plugins/com-artemisoftnian-plugins-unityads2/test/* www/;

	# now build and run the demo in your device or emulator
    cordova prepare; 
    cordova run android; 
    cordova run ios;
    # or import into Xcode / eclipse
```

## INSTALLATION

* If use with Cordova CLI:
```bash
cordova plugin add com-artemisoftnian-plugins-unityads2
```

* Using NPM
npm install com-artemisoftnian-plugins-unityads2


## USAGE

Show Mobile Ad with single line of javascript code.

Step 1: Create a new project for the desire platform in [UnityAds portal](https://operate.dashboard.unity3d.com), then write it in your javascript code.

```javascript
// select the right Ad Id according to platform
var gameId = "Android or iOS Game ID";
var videoAdPlacementId = "Video Placement ID";
var rewardedVideoAdPlacementId = "Rewarded Placement ID";
```

Remember to put `isTest = false` when building for production.

## METHODS

```javascript
// Initialize UnityAds
UnityAdsInit(gameId, isTest, isDebug, fn);

// Video Ads Related (Regular/Rewarded)
ShowVideoAd(videoPlacementId, fn);
GetPlacementState(videoAdPlacementId, fn);


## Screenshots

Android Video Ads

![ScreenShot](https://github.com/artemisoftnian/com-artemisoftnian-plugins-unityads2/raw/master/doc/android/android_1.png)
![ScreenShot](https://github.com/artemisoftnian/com-artemisoftnian-plugins-unityads2/raw/master/doc/android/android_2.png)
![ScreenShot](https://github.com/artemisoftnian/com-artemisoftnian-plugins-unityads2/raw/master/doc/android/android_3.png)

iOS Video Ads
![ScreenShot](https://github.com/artemisoftnian/com-artemisoftnian-plugins-unityads2/raw/master/doc/ios/ios_1.png)
![ScreenShot](https://github.com/artemisoftnian/com-artemisoftnian-plugins-unityads2/raw/master/doc/ios/ios_2.png)
![ScreenShot](https://github.com/artemisoftnian/com-artemisoftnian-plugins-unityads2/raw/master/doc/ios/ios_3.png)


* Important DONT GET BANNED: Please read carfully the [Unity Monetization Services Terms of Service](https://unity3d.com/legal/monetization-services-terms-of-service).


## Credits

This project is created and maintained by Waldemar Medina.
Available for project outsourcing and or consulting services. [Lets Talk](mailto:waldemar_medina@hotmail.com) I can help in your project.

## Donations

If this project help you reduce time to develop, or You simple found it usefull please consider give me a cup of coffee. I like pizza too :)

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4RK9RWFNTBNUA)