# My Day — Android project

This is a native Android WebView wrapper around the My Day V1.1 HTML prototype.

## Build
1. Open this folder as a project in Android Studio on a computer.
2. Let Gradle sync.
3. Build > Build APK(s).
4. Install the generated debug APK on your Android phone.

## Current contents
- Existing My Day HTML prototype bundled locally in `app/src/main/assets/index.html`
- WebView launcher activity
- Notification permission/channel
- WorkManager hourly motivation reminders, intended for 8 AM–10 PM

## Important limitations
- This ZIP is source code, not an APK.
- A Gradle/Android build environment is required to compile it; Android Studio is the easiest supported route. A phone-only cloud build needs a compatible service and may require uploading the project ZIP.
- WorkManager periodic work is inexact. Android may delay hourly reminders, and manufacturer battery restrictions can delay them further. This is not an exact alarm.
- Prototype data is stored by the WebView in local storage; uninstalling/clearing app data can remove it.
- The app's Isha date boundary remains based on the prototype's manually configured Isha time.
- Review permissions and test notifications on the target Android version before relying on reminders.
