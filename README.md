# THE FORGOTTEN Modeler — Android project

This project wraps the existing Modeler v5 web app in an Android WebView.

## Important
- This ZIP is source code, **not an APK**.
- The app loads `index.html` from Android assets. The 3D app currently loads Three.js from a CDN, so an internet connection may be required.
- It has not been tested on a physical Android device.
- Application ID: `com.theforgotten.modeler`; minimum Android API: 23 (Android 6.0).

## Build in Android Studio
Open the project and run `gradle assembleDebug` or use **Build > Build Bundle(s) / APK(s) > Build APK(s)**.

## Cloud build workflow
The `.github/workflows/build-apk.yml` workflow is included for GitHub Actions. Once this project is placed in a GitHub repository, open **Actions**, select **Build THE FORGOTTEN Modeler APK**, and run the workflow. When it finishes, open the run and download the artifact named `THE-FORGOTTEN-Modeler-debug-APK`. Extract the artifact ZIP to get `app-debug.apk`.

The cloud workflow is provided but has not been run from this environment, so the APK build is not yet verified.
