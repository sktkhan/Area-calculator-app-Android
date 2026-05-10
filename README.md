# Area Calculator App - Android

A simple yet powerful Android application for calculating the area of different geometric shapes. Built with Android Studio and the latest Android development practices.

## Features

- 📐 **Calculate areas for:**
  - Rectangle (Length × Width)
  - Circle (π × r²)
  - Triangle (½ × Base × Height)

- 🎨 **Modern UI Design** with smooth animations and intuitive interface
- 🔐 **Privacy-Focused** - No data collection or tracking
- 📱 **Responsive Design** - Works on all Android devices
- ⚡ **Fast & Lightweight** - Minimal resource usage

## Project Structure

```
Area-calculator-app-Android/
├── app/
│   ├── build.gradle                    # App-level build configuration
│   ├── proguard-rules.pro             # ProGuard rules for code shrinking
│   └── src/
│       └── main/
│           ├── AndroidManifest.xml    # App manifest
│           ├── assets/
│           │   ├── calculator.html    # Calculator UI (HTML/CSS/JS)
│           │   └── privacy_policy.html # Privacy policy page
│           ├── java/com/akhtar/areacalculator/
│           │   ├── MainActivity.java
│           │   └── PrivacyPolicyActivity.java
│           └── res/
│               ├── layout/
│               │   ├── activity_main.xml
│               │   └── activity_privacy_policy.xml
│               ├── values/
│               │   ├── strings.xml
│               │   ├── colors.xml
│               │   └── themes.xml
│               ├── drawable/
│               │   └── ic_launcher_foreground.xml
│               ├── menu/
│               │   └── main_menu.xml
│               ├── mipmap-*/
│               │   ├── ic_launcher.xml
│               │   └── ic_launcher_round.xml
│               └── xml/
│                   └── network_security_config.xml
├── gradle/
│   └── wrapper/
│       └── gradle-wrapper.properties
├── build.gradle                       # Root build configuration
├── settings.gradle                    # Project settings
├── gradle.properties                  # Gradle properties
├── gradlew                           # Gradle wrapper script
└── .github/workflows/
    └── build.yml                     # GitHub Actions CI/CD

```

## Requirements

- Android API 21+ (Android 5.0 - Lollipop)
- Java 11+
- Gradle 8.4+

## Building the Project

### Using Gradle Wrapper

```bash
# Make gradlew executable (if on Unix/Linux/Mac)
chmod +x gradlew

# Build Debug APK
./gradlew assembleDebug

# Build Release APK
./gradlew assembleRelease

# Run Tests
./gradlew test
```

### APK Location

After building, the APK files will be located at:
- **Debug APK:** `app/build/outputs/apk/debug/app-debug.apk`
- **Release APK:** `app/build/outputs/apk/release/app-release.apk`

## Technologies Used

- **Language:** Java
- **Build System:** Gradle 8.4
- **Android Framework:** AndroidX
- **UI:** XML Layouts + WebView with HTML/CSS/JavaScript
- **Target SDK:** 34 (Android 14)
- **Minimum SDK:** 21 (Android 5.0)

## Privacy Policy

This app respects user privacy:
- ❌ No personal data collection
- ❌ No analytics or tracking
- ❌ No ads or third-party services
- ✅ All calculations are local to the device

See [Privacy Policy](app/src/main/assets/privacy_policy.html) for more details.

## GitHub Actions Workflow

The project includes automated CI/CD using GitHub Actions:
- Automatic APK builds on push to main branch
- Manual workflow dispatch available
- Built APK artifacts retained for 60 days

## License

This project is available for personal and educational use.

## Author

Created by Akhtar Khan

## Version

- **Version:** 1.0
- **Last Updated:** January 2026
