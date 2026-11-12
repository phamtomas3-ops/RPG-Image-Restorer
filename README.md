# RPG Image Restorer

An offline Android app for restoring encrypted RPG Maker image assets to standard PNG files.

## Features

- Restore RPG Maker `.png_` image files.
- Select individual files or scan a folder.
- Batch conversion with per-file status and progress.
- Cancel a running batch.
- Choose an output folder with Android's document picker.
- Preview and share restored images.
- Export converted images as a ZIP archive.
- Dark Material 3 interface.
- On-device processing; conversion does not require an internet connection.

## Installation

1. Open the [Releases](https://github.com/phamtomas3-ops/RPG-Image-Restorer/releases) page.
2. Download the APK attached to the release.
3. Open the APK on your Android device and follow Android's installation prompts.

## Usage

1. Open RPG Image Restorer.
2. Select one or more `.png_` files, or choose a folder to scan.
3. Select an output folder.
4. Start the conversion.
5. Review the results and save, ZIP, or share the restored images.

## Supported formats

- **`.png_`:** primary target; test with files from games you are authorized to use.
- **`.rpgmvp`:** accepted by the folder scanner, but restoration compatibility has not yet been verified.

Compatibility can vary with RPG Maker version and encryption format. This is an early release, so please report failures with a sample file you have permission to share and the error message shown by the app.

## Building from source

The project is an Android/Kotlin Gradle project.

1. Clone this repository.
2. Extract `RpgImageRestorer.zip` from the repository.
3. Open the extracted project directory in Android Studio.
4. Allow Gradle to sync, then run the `assembleDebug` task.

A GitHub Actions workflow is provided to build a debug APK in the cloud. Download the APK from the workflow run's **Artifacts** section.

## Privacy

Image conversion is performed locally on your device. The app uses Android's Storage Access Framework for file selection and output access rather than requesting broad storage permissions.

## Credits and acknowledgements

The restoration behavior was developed with the [Petschko RPG Maker MV Decrypter](https://petschko.org/tools/mv_decrypter/index.html#restore-images) as a reference.

RPG Maker is a trademark of its respective owner. This is an independent community project and is not affiliated with or endorsed by RPG Maker or its developers.

## Project status

**Early testing release.** The initial Android build has been produced, but compatibility with all RPG Maker image formats and game versions has not been established.
