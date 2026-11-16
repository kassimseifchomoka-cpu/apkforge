# APKFORGE v1.0.3
APKFORGE is a web APK package inspector plus a native Android companion shell.

## What works in this source package
- Browser-local APK intake, ZIP signature check, file size and SHA-256.
- No APK upload: inspection happens locally in the browser.
- Android WebView companion app source.
- GitHub Actions workflow to compile a debug APK and publish it as an artifact.

## Honest limits
This is not a compiler for arbitrary APKs and does not convert arbitrary files into apps. It does not scan for malware or guarantee installability. It does not re-sign third-party APKs. DLS26 is not included; the owner must supply the legitimate test APK.

## Web version
Open `index.html`, or deploy the repository with GitHub Pages (Settings → Pages → Deploy from branch → main / root).

## Android build
Push this project to GitHub. The workflow `.github/workflows/android.yml` builds `android/app/build/outputs/apk/debug/app-debug.apk`. Download it from Actions → workflow run → Artifacts.

Package id: `com.chomz.apkforge`
