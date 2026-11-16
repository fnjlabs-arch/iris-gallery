<p align="center">
  <img src="fastlane/metadata/android/en-US/images/icon.png" width="112" height="112" alt="SadSha Gallery" style="border-radius: 24px;" />
</p>

<h1 align="center">SadSha Gallery</h1>

<p align="center">
  A fast, private, 100% offline gallery app for Android built with Jetpack Compose and Material 3.
</p>

<p align="center">
  <b>SadSha Gallery</b> is a SadSha rebrand of <a href="https://github.com/MohamadOday/iris-gallery">Iris Gallery</a> by Mohamad Oday, licensed under the Apache License 2.0.<br/>
  Package <code>com.sadsha.gallery</code> · SadSha amber theme · Free v1, no account, no ads.
</p>

---

> [!CAUTION]
> **Dev Notice**
> 
> We do not welcome contributions, collaboration, or support from individuals, companies, or organizations that justify, stand , defend or participate with/in Israeli war crimes, illegal settlement expansion, interventions , actions , or apartheid . 
> 
> Stand for justice, or do not stand with this project.

---

<p align="center">
  <img src="fastlane/metadata/android/en-US/images/phoneScreenshots/1_photos_timeline.png" width="18%" />
  <img src="fastlane/metadata/android/en-US/images/phoneScreenshots/2_albums_grid.png" width="18%" />
  <img src="fastlane/metadata/android/en-US/images/phoneScreenshots/4_photo_viewer.png" width="18%" />
  <img src="fastlane/metadata/android/en-US/images/phoneScreenshots/5_photo_editor.png" width="18%" />
  <img src="fastlane/metadata/android/en-US/images/phoneScreenshots/8_app_lock.png" width="18%" />
</p>

SadSha Gallery is designed to be a private, responsive, and customizable local media viewer. It has zero network permissions, opens instantly, and stays out of your way.

## Download & Installation

Test APK (debug build, phone test only — not for Play Store):

- https://pub-a7c575ef05cf4d448836863e0ceb44c8.r2.dev/sadsha-gallery-test.apk

Or build from source (see below). The Play Store release build (AAB) needs the SadSha release keystore — see `.github/workflows/build-release-aab.yml`.

Upstream releases of the original app live at [MohamadOday/iris-gallery](https://github.com/MohamadOday/iris-gallery/releases/latest).

---

## Highlights

- **100% Offline & Private**: Zero `INTERNET` permission in the manifest. Photos, videos, and metadata never leave your device.
- **Live Media Sync**: Automatic real-time timeline detection for new camera photos and downloads without needing app restarts.
- **Fluid Grid & Pinch Resize**: Smoothly resize the photos grid (2–6 columns) and albums grid (1–4 columns) with responsive pinch gestures.
- **Built-in Photo Editor**: Crop with aspect presets, rotate, flip, adjustments (Brightness, Contrast, Saturation, Warmth), freehand blur/pixelate brushes, resize, and external editor integration (Snapseed, Lightroom, ImageToolbox).
- **High-Res Viewer & EXIF/GPS Inspector**: Hardware canvas rendering with multi-level zoom (up to 7×), detailed camera metadata (ISO, aperture, shutter speed, focal length), and one-tap map location launcher.
- **Media3 Video Player**: Powered by ExoPlayer with sensor-aware hardware rotation, gesture seeking, auto-play, and mute controls.
- **App Lock & Private Vault**: Protect the entire app or media picker with a custom PIN and biometric fingerprint unlock, plus a dedicated encrypted vault for sensitive media.
- **Safe 30-Day Trash**: Move deleted items to the trash with easy restoration or one-tap permanent purge.
- **Album Management**: Create custom albums, move/copy media between folders, customize album covers, pin favorites, and sort by name, date, or count.
- **Duplicate & Similar Photo Finder**: Scan and clean up redundant media to reclaim device storage.
- **Smart Media Categorization**: Dedicated filters for RAW photos, animated GIFs, Motion Photos, Panoramas, and Screenshots.
- **Home Screen Photo Widget**: Customizable home screen widget with automatic memory rotation.
- **Multilingual Support**: Fully localized in 13+ languages with in-app language switcher.
- **Deep Customization**: Material You dynamic theming, pure AMOLED dark mode, adjustable corner rounding, startup tab selection, and thumbnail grid density sliders.

## Building

### Requirements
- Android SDK 35+ / Build-Tools 36.0.0+
- JDK 17+

### Build from source

```bash
git clone https://github.com/fnjlabs-arch/iris-gallery.git
cd iris-gallery

# Build debug APK
./gradlew assembleDebug

# Build release APK
./gradlew assembleRelease
```

The APK will be generated under `app/build/outputs/apk/`.

## Privacy

SadSha Gallery does not include any analytics, crash reporters, telemetry, or network-enabled libraries. The app cannot make network requests at runtime because network permissions are completely omitted from `AndroidManifest.xml`.

## Upstream credit

SadSha Gallery is based on [Iris Gallery](https://github.com/MohamadOday/iris-gallery) by Mohamad Oday, licensed under the Apache License 2.0 (see `LICENSE`). The original app is also on [F-Droid](https://f-droid.org/packages/com.iris.gallery/). This fork only rebrands it (name, package, icon, SadSha amber theme) and adds CI build workflows; all features are the upstream app's work.

## License

```
Copyright 2026 Mohamad Oday

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
