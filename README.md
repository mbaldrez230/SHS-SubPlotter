# SHS SubPlotter (Android)

Reads the public Google Sheet "LNHS-SHS-SUBSTITUTION-FORM (Responses)"
(Timestamp, NAME, DATE, TIMESLOT, SUBJECT, SECTION, SUBSTITUTE, REASON OF ABSENCE).

- Top bar (#0437F2): logo (tap = Settings), app name, Search, Refresh.
- Weekly calendar by default (monthly in Settings). Tap the month or year label to jump to another month/year.
  Today = blue, upcoming days with entries = yellow fill, past days with entries = yellow frame.
- Dashboard (below the calendar): date + filter icon (filters the displayed day by NAME / SECTION / RELIEVER).
  Cards show TIMESLOT, RELIEVER, SUBJECT, SECTION; tap a card for the full details.
- Search (NAME / RELIEVER): results pop-up with a category dropdown (TODAY / THIS WEEK / THIS MONTH / THIS YEAR / ALL).
  Tap a result for the full details.
- Settings: ADD ENTRIES (opens the Google Form), calendar view, auto-update (off / 30 s / 1 / 5 / 15 / 30 min),
  change Google Form and Google Sheet (password: lnhs-shs-la-union). Everything is saved on the device.

## Logo
The logo is downloaded once from the link you gave and cached on the phone.
For a guaranteed offline logo, save your image as app/src/main/res/drawable-nodpi/app_logo.png before building.

## Get the APK
A) Android Studio: open this folder, let Gradle sync, Build > Build APK(s).
   Output: app/build/outputs/apk/debug/app-debug.apk
B) GitHub Actions: upload this folder to a GitHub repo, Actions > "Build APK" > Run workflow,
   then download the "SubstituteDashboard-APK" artifact.
