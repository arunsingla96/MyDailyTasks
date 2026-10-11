# Build your APK online (no Android Studio needed)

This project includes a GitHub Actions workflow that builds a debug APK in the cloud.

## Steps
1. On your phone, open https://github.com and sign in or create a free account.
2. Create a new repository. Name it `MyDailyTasks`. Choose **Private** if you prefer, then create it.
3. Open the new repository and choose **Add file → Upload files**.
4. On your phone, extract this ZIP first using your Files app. Open the extracted `MyDailyTasks` folder and upload its contents (including the hidden `.github` folder if your file picker permits it). If uploading folders/hidden files is difficult on mobile, use a computer or a GitHub-compatible upload client.
5. Commit the uploaded files to the `main` branch.
6. Open the repository's **Actions** tab. Select **Build My Daily Tasks APK**. If prompted, enable workflows, then tap **Run workflow**.
7. Wait for the run to finish with a green check. Open that run, scroll to **Artifacts**, and download `MyDailyTasks-debug-apk`.
8. Extract the downloaded artifact ZIP; it contains `app-debug.apk`. Tap the APK to install it. Android may ask you to allow installs from that source; only enable this for the browser/files app you used, and turn it off again afterward if desired.

## Important
- This produces a **debug APK** for personal testing, not a Play Store release.
- Android may require notification permission and exact-alarm permission/settings for reminders. Battery optimization or manufacturer restrictions can affect alarm delivery. Test a reminder shortly in the future before relying on it.
- This workflow has not yet been run against GitHub Actions, so a successful build is not guaranteed until the first run completes. If it fails, open the failed run's log and share the error text so it can be fixed.
