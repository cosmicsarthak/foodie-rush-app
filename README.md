# Foodie Rush App

Food Delivery App built using **Flutter** - _Android_

#### ⚓Tech Stack

- Flutter `Dart`
- Firebase
- Firestore
- BloC
- Hive

> check flutter support: `flutter doctor`

---

### ⏬Get all Packages

```dart
flutter pub get
```

```dart
flutter pub update
```

### ▫️▫️▫️ Run the App

```dart
flutter run <DART_FILE>
```

### Testing

```dart
flutter test [<DIRECTORY|DART_FILE>]
```

### If getting errors

```dart
flutter logs
```

---

## To Deploy & Sign the App

### Create an upload keystore

```shell
  keytool -genkey -v -keystore ~/upload-keystore.jks -keyalg RSA \
          -keysize 2048 -validity 10000 -alias upload
```

OR

```shell
  keytool -genkey -v -keystore %userprofile%\upload-keystore.jks ^
          -storetype JKS -keyalg RSA -keysize 2048 -validity 10000 ^
          -alias upload

```

### Reference the keystore from the app

> From DOCS

- Create a file named [project]/android/key.properties that contains a reference to your keystore. Don’t include the angle brackets (< >). They indicate that the text serves as a placeholder for your values.

```
content_copy
storePassword=<password-from-previous-step>
keyPassword=<password-from-previous-step>
keyAlias=upload
storeFile=<keystore-file-location>
```

> also can refer: https://docs.flutter.dev/deployment/android#configure-signing-in-gradle

### Releasing the App on Platforms

- [official guide on App Release](https://docs.flutter.dev/deployment/android#build-an-app-bundle)

## Admin App

> [Admin App Repository](https://github.com/cosmicsarthak/foodie_rush_admin)

---

[👋 `Sarthak Mohanty`](https://sarthak.app)
