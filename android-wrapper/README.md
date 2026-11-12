# NEXTY MINE Android wrapper

This folder builds a simple Android shell that loads the existing NEXTY MINE website:
https://nextystudio1.github.io/NEXTY-MINE/

## Build a test APK
1. Open the repository on GitHub.
2. Go to Actions.
3. Select **Build NEXTY MINE Android APK**.
4. Select **Run workflow** and confirm.
5. When the workflow finishes, open its run and download the `nexty-mine-debug-apk` artifact.

The generated APK is a **debug/test build** signed with the Android debug key. It is for installation testing only, not a final store release. A production release must be built and signed with a private release keystore, which should be created and kept by the adult account owner/publisher. Never commit a keystore or passwords to this repository.

The Android app loads the live website, so an internet connection is required. Game logic, accounts, and data remain on the existing website and Supabase backend.
