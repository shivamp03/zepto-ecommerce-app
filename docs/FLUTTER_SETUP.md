# Flutter Setup Guide

## Prerequisites

- Flutter SDK 3.0 or higher
- Dart SDK (comes with Flutter)
- Android Studio or Xcode
- An Android device or emulator / iOS simulator

## Installation Steps

### 1. Install Flutter

```bash
# Download Flutter SDK from https://flutter.dev/docs/get-started/install
# Add Flutter to your PATH

# Verify installation
flutter doctor
```

### 2. Create Flutter Project

```bash
cd flutter_app
flutter pub get
```

### 3. Configure Firebase

#### For Android:
1. Create a Firebase project at [Firebase Console](https://console.firebase.google.com)
2. Add an Android app to your project
3. Download `google-services.json` and place it in `android/app/`
4. Follow Firebase setup instructions

#### For iOS:
1. Add an iOS app to your Firebase project
2. Download `GoogleService-Info.plist` and add it to Xcode project
3. Follow Firebase setup instructions

### 4. Add Dependencies

Key dependencies to add to `pubspec.yaml`:

```yaml
dependencies:
  flutter:
    sdk: flutter
  firebase_core: ^latest
  firebase_auth: ^latest
  cloud_firestore: ^latest
  http: ^latest
  provider: ^latest
  get: ^latest
  shared_preferences: ^latest
  intl: ^latest
```

### 5. Project Structure

```
flutter_app/
├── lib/
│   ├── main.dart
│   ├── models/
│   │   ├── user_model.dart
│   │   ├── product_model.dart
│   │   └── order_model.dart
│   ├── screens/
│   │   ├── auth/
│   │   ├── home/
│   │   ├── products/
│   │   ├── cart/
│   │   └── profile/
│   ├── services/
│   │   ├── auth_service.dart
│   │   ├── api_service.dart
│   │   └── firestore_service.dart
│   ├── widgets/
│   │   ├── custom_app_bar.dart
│   │   ├── product_card.dart
│   │   └── bottom_nav.dart
│   └── utils/
│       ├── constants.dart
│       └── themes.dart
├── assets/
│   ├── images/
│   └── icons/
├── android/
├── ios/
└── pubspec.yaml
```

## Running the App

```bash
# Run on emulator/device
flutter run

# Run with specific device
flutter devices
flutter run -d <device_id>

# Build APK
flutter build apk

# Build iOS
flutter build ios
```

## Development Tips

- Use hot reload: Press `r` in terminal
- Use hot restart: Press `R` in terminal
- Enable verbose logging: `flutter run -v`
- Run tests: `flutter test`

## Troubleshooting

- Run `flutter clean` if you face build issues
- Update dependencies: `flutter pub upgrade`
- Check Firebase configuration is correct
