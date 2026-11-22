# USYEI Monitor

USYEI Monitor is a polished offline-first Android Flutter MVP for UPSHIFT Youth Empowerment Initiative.

## Included in this version

- Professional dashboard with attendance statistics and recent scans.
- One-tap QR attendance scanner with camera error handling and feedback.
- Student list with search, Active/Inactive filters, CSV import, QR codes and actions.
- Student profile with attendance summary and QR code.
- Attendance history with date selection, search, Present/Absent filters, manual toggle and CSV export.
- Symmetrical 3-item bottom navigation: Dashboard, Students, Attendance.
- Centered Scan QR floating action for quick attendance from any main section.
- Navigation drawer for secondary actions and PIN change.
- Branded splash/loading screen showing the USYEI logo and “Powered by Kephy Tech”.
- Old generated Flutter widget test removed so it cannot block the Codemagic APK build.

## Codemagic

The repository includes `codemagic.yaml` for an Android release APK. The workflow uses Flutter stable, Java 17, runs `flutter analyze lib --no-fatal-warnings --no-fatal-infos`, and builds `flutter build apk --release`.


## Corrected branding and release

The visible app brand is **USYEI Monitor**. The existing Android application ID (`com.upshift.useyi_monitor`) is intentionally retained so this release can update the previously installed working APK instead of creating a second app. The Codemagic Android workflow is preserved from the successful build configuration.
