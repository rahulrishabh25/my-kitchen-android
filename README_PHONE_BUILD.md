# My Kitchen — Made by Rahul

Android WebView wrapper project for the My Kitchen mobile-first app prototype.

## Build an installable APK using only an Android phone

This project includes a GitHub Actions workflow that builds a **debug APK** in the cloud. You do not need Android Studio or a laptop.

1. In your phone browser, sign in to GitHub and create a **new public or private repository** named `my-kitchen`.
2. Upload the contents of this project to the repository, preserving the folder structure. The `.github/workflows/build-apk.yml` file is essential. If GitHub's mobile uploader cannot preserve folders, use GitHub's browser desktop mode or GitHub Codespaces.
3. Open the repository's **Actions** tab and select **Build My Kitchen APK**. Tap **Run workflow** (or push/upload to `main` to trigger it automatically).
4. Wait for the workflow to finish successfully.
5. Open the completed workflow run, scroll to **Artifacts**, and download `My-Kitchen-APK`. Extract the ZIP on your phone to get `app-debug.apk`.
6. Tap the APK and follow Android's install prompt. If needed, allow your browser or file manager to install unknown apps, then turn that permission off again afterward.

## What's included
- WebView Android app wrapper
- Local HTML app bundled offline
- JavaScript and local storage enabled
- Image picker support for adding item photos
- Cloud build workflow that outputs a debug APK

## Important feature limits
The included web prototype stores data locally on one device/browser. It has pantry and fridge items, quantity and expiry tracking, favourite recipes, frequent-item sorting, recipe ingredient availability, item/restock sharing, and export/import backup. Browser notifications are not guaranteed while the app is closed. Household code/QR and export/import do not provide secure real-time family sync. A production release needs native scheduled notifications and a secure shared backend (for example Firebase) before relying on family access.

The APK produced by this workflow is a **debug APK** suitable for personal testing, not a Play Store release. It is not release-signed.
