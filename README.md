# CharityApp

Android application for charity management and donations.

## Status

This repository is a fork of [`JstMagic/charityapp`](https://github.com/JstMagic/charityapp). The codebase still uses an older Android toolchain and Firebase setup, so contributors should expect some modernization work before targeting current Android versions.

## What The App Includes

- User authentication: login, sign up, forgot password
- Charity management: stories, staff, updates
- Donation flow and donation details
- User profiles and contributor details
- Notifications and media content screens

## Project Structure

The source code is organized under `app/src/main/java/com/kodemakers/charity/`:

```text
activities/    Screens and flows
adapter/       RecyclerView adapters
app/           Application-wide config
custom/        Helpers, networking, storage utilities
fonts/         Custom text widgets
model/         Response and domain models
service/       Firebase and notification services
```

## Prerequisites

- Android Studio
- JDK compatible with Android Gradle Plugin `3.3.2`
- A Firebase project for `com.kodemakers.charity`

## Local Setup

1. Clone your fork:

```bash
git clone https://github.com/<your-github-username>/charityapp.git
cd charityapp
```

2. Add Firebase config:
   Place your own `google-services.json` file in `app/google-services.json`.

3. Open the project in Android Studio and let Gradle sync.

4. Run the `app` configuration on an emulator or device.

## Secrets And Local Files

This repo does not track signing keys or Firebase config anymore.

- Keep keystores out of version control.
- Keep `google-services.json` local to your machine.
- Use Android Studio's default debug signing for local development.

## Notable Technical Details

- Language: Java
- Package: `com.kodemakers.charity`
- Gradle wrapper: `4.10.1`
- Android Gradle Plugin: `3.3.2`
- `compileSdkVersion` / `targetSdkVersion`: `27`

## Contribution Ideas

- Upgrade Gradle, Android Gradle Plugin, and SDK targets
- Replace deprecated Firebase Instance ID usage
- Remove legacy storage assumptions for newer Android versions
- Add setup validation and clearer error handling around Firebase-dependent flows
- Add contributor docs and screenshots

## Upstream

- Fork: https://github.com/Farukhsb/charityapp
- Original project: https://github.com/JstMagic/charityapp
