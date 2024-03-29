# Android VCS Realtime SDK

## Description

This is the Android library for the VCS Realtime SDK. This library can be included in an Android project to provide support for joining virtual rooms and interacting with audio and/or video.

Where to find more information about the VCS Realtime SDKs and APIs.

* For more information on the VCS SDK family, see the [VCS realtime SDK page](https://sdk.virtualcareservices.net/)
* For more information on the VCS Android SDK, see the [guide for Android realtime SDK](https://sdk.virtualcareservices.net/sdks/android)
* A list of all APIs for the Android SDK is available at the [reference API for Android realtime SDK](https://sdk.virtualcareservices.net/reference/android)
* A sample app for the Android SDK is available [here](https://github.com/ATOS-VIRTUAL-CARE/vcs-realtime-sdk-android-demo)


## Integrate Into Android Project
Add the Android SDK and WebRTC image repositories to the root gradle file:
```xml
...
allprojects {
    repositories {
        ...
        maven { url 'https://raw.github.com/ATOS-VIRTUAL-CARE/vcs-realtime-sdk-android/repo/' }
        maven { url 'https://raw.github.com/ATOS-VIRTUAL-CARE/webrtc-android/repo/' }
    }
}
```

Add the following dependencies to your app module (such as app/build.gradle) and update the version to the latest releases. The apollo runtime will also need to be added as a dependency; the current version the SDK is using is 3.2.2.
```xml
dependencies {
    ...
    implementation 'atos.virtual.care:vcs-reatime-sdk:x.x.x'
    implementation 'atos.virtual.care:libwebrtc:M102'
    implementation 'com.apollographql.apollo3:apollo-runtime:3.2.2'
}
```

