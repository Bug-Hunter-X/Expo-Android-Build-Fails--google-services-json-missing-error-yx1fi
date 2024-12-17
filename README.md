## Expo Android Build Failure: Missing google-services.json

This repository demonstrates a common error encountered when building Android APKs using the Expo CLI.  Despite having the `google-services.json` file in the expected location (`android/app`), the build process fails with a "missing file" error. This issue often arises from incorrect file placement or multiple `google-services.json` files in the project structure. The solution involves ensuring only one `google-services.json` exists in the `android/app` directory and resolving any potential conflicts.

### Steps to Reproduce:

1. Clone this repository.
2. Attempt to build the Android APK using `expo build:android`.
3. Observe the build failure with the "missing google-services.json" error message.

### Solution:

The `bugSolution.js` file provides a corrected project structure and demonstrates the necessary steps to resolve the conflict by ensuring only one valid `google-services.json` file is in the `android/app` directory.