# INDIALINK — Google Play release checklist

## Build
- Package: `com.indialink.patient`
- Version: `1.0.0`
- Version code: `1`
- Minimum Android: API 24 (Android 7.0)
- Target Android: API 36 (Android 16)
- Play upload format: Android App Bundle (`.aab`)

## GitHub Actions secrets
Add these repository secrets before running **Build Play Store Release**:
- `ANDROID_KEYSTORE_BASE64`
- `ANDROID_KEYSTORE_PASSWORD`
- `ANDROID_KEY_ALIAS`
- `ANDROID_KEY_PASSWORD`

Never commit the keystore or signing passwords to the repository.

## Play Console
1. Create/verify an Organization developer account.
2. Create the app with package `com.indialink.patient`.
3. Enroll in Google Play App Signing.
4. Upload `INDIALINK-Patient-v1.0.0.aab`.
5. Complete App access, Ads, Content rating, Target audience, Data safety and Health apps declaration.
6. Add the public privacy policy URL.
7. Complete store listing assets and testing/release tracks.

## Product note
This project currently uses a WebView-based shell around the INDIALINK patient website. Before production submission, add meaningful native/app-specific functionality and thoroughly test the mobile UX, because Google Play requires stable and sufficiently useful app experiences.
