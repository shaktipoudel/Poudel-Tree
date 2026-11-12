# Family Tree Android App

A simple offline Android app for adding and editing family members and their relationships.

## Features
- Add, edit and delete family members
- Define relationships (father, mother, husband, wife, son, daughter, brother, sister, grandparents, other)
- Link each person to an existing family member
- Store data locally on the device using SharedPreferences
- Build an APK using GitHub Actions

## Build on GitHub
1. Create a new GitHub repository.
2. Upload the contents of this folder to the repository root (not the ZIP file itself).
3. Commit to the `main` branch.
4. Open **Actions** and select **Build Family Tree APK**.
5. Wait for the workflow to finish successfully.
6. Open the workflow run, scroll to **Artifacts**, and download `FamilyTree-debug-apk`.
7. Extract the downloaded artifact to get `app-debug.apk`.

You can also run the workflow manually from **Actions → Build Family Tree APK → Run workflow**.

## Build locally
Requires JDK 17 and Gradle 8.7:
```bash
gradle assembleDebug
```
APK output: `app/build/outputs/apk/debug/app-debug.apk`

## Notes
- This is a debug APK for testing and personal use.
- App data is stored locally on the device; uninstalling the app may remove it.
- A member can be linked to one related person. For complex family structures, add additional relationship records in a future version.
