# Build WakaûndūVibez Studio using only your phone

This project ZIP includes a GitHub Actions workflow that can build a debug APK in the cloud.
You do not need Android Studio installed on your phone, but you do need a GitHub account and an internet connection.

## Steps

1. Download and extract this ZIP using your phone's Files app. If your phone cannot extract ZIP files, install a trusted archive app from Google Play.
2. In your phone browser, sign in at https://github.com and create a **new public or private repository**. Do not add a README or license during repository creation.
3. Upload the *contents* of the extracted project folder to the repository root. Make sure the `.github/workflows/android-apk.yml` file is included. On GitHub's mobile website, use **Add file → Upload files** if available. Some mobile browsers hide dot-folders; if `.github` cannot be uploaded, switch the browser to desktop site or use GitHub's mobile app/browser desktop mode.
4. Commit the uploaded files to the `main` branch.
5. Open the repository's **Actions** tab, select **Build Android APK**, and choose **Run workflow** if it has not started automatically. Confirm by tapping **Run workflow**.
6. Wait for the workflow to finish successfully. Open that run, scroll to **Artifacts**, and download `WakaudVibezStudio-debug-apk`.
7. Extract the downloaded artifact ZIP. Tap the `.apk` file to install it. Android may ask you to allow your browser or Files app to install unknown apps; only enable this for the app you are using to install this APK, then turn it off again afterward.

## Important notes

- This produces a **debug APK**, not a Play Store release.
- The build has not been verified on a physical device. If the workflow fails, open the run's build log and use the error message to fix the project before retrying.
- Never upload passwords, signing keys, API keys, or private personal data to the repository.
