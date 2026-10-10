# My Exam Planner — Android app project

This Android app wraps the latest My Exam Planner interface in an offline WebView, preserving the existing design and features rather than rebuilding a simplified planner.

## Included features
- Same My Exam Planner UI and colors
- Monday–Sunday plans and checklists
- Live completion counters and weekly progress
- Master To Do and Notes (Weekly Intentions is not present)
- Save Weekly Plan, weekly navigation, saved-week history, reset
- Custom colors and WhatsApp sharing
- Automatic on-device saving through WebView local storage
- Works offline; no account and no app server required

## Build an installable APK
This workspace does not have the Android SDK or Gradle installed, so an APK could not be compiled here. The project includes a GitHub Actions workflow to build it for you:

1. Download and extract this project ZIP on a computer.
2. Create a new repository on GitHub and upload the extracted files.
3. Open the repository's **Actions** tab and choose **Build My Exam Planner APK**.
4. Click **Run workflow** (if it has not run automatically).
5. When the workflow finishes, download the **My-Exam-Planner-APK** artifact from the run. Extract it to get `app-debug.apk`.
6. Transfer `app-debug.apk` to your Android phone, tap it, and allow your file manager to install unknown apps if Android asks.

Alternatively, open the project folder in Android Studio and choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**. Install `app/build/outputs/apk/debug/app-debug.apk` on your phone.

## Data and privacy
Planner data is stored locally on the phone in the app's WebView storage. It is not uploaded to a server. Uninstalling the app or clearing its app storage can erase saved planner data. WhatsApp sharing opens the external WhatsApp/link handler only when you tap Share.
