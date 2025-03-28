# Deployment Guide

## Prerequisites
- Android Studio 2022.3+
- Java 17+
- Android SDK 34
- Google Play Developer Account

## Build Process
1. Configure signing in `app/build.gradle`:
```gradle
android {
    signingConfigs {
        release {
            storeFile file("keystore.jks")
            storePassword "password"
            keyAlias "key0"
            keyPassword "password"
        }
    }
}
```

2. Build release APK:
```bash
./gradlew assembleRelease
```

3. Generate App Bundle:
```bash
./gradlew bundleRelease
```

## Play Store Submission
1. Create new release in Play Console
2. Upload signed App Bundle
3. Add release notes
4. Upload screenshots (min 2 per device type)
5. Submit for review

## Version Management
- Update in `app/build.gradle`:
```gradle
defaultConfig {
    versionCode 2
    versionName "1.0.1"
}