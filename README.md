# HABIT TRACKER x FLUTTER
 **Steps to be followed**
 # Setting Up Android Studio for Flutter Development

Follow these steps to configure Android Studio for running Flutter apps on your machine.

## Prerequisites

1. **Install Flutter:**
   - Follow the [official Flutter installation guide](https://flutter.dev/docs/get-started/install) to download and set up Flutter on your machine.

2. **Install Android Studio:**
   - Download and install [Android Studio](https://developer.android.com/studio), which includes the Android SDK.

## Setup Steps

### 1. Install Flutter and Dart Plugins:

- Open Android Studio.
- Go to "Preferences" (on macOS) or "Settings" (on Windows/Linux).
- Select "Plugins" in the left sidebar.
- Search for "Flutter" and "Dart" plugins.
- Click "Install" for both plugins.

### 2. Configure Flutter SDK Path:

- In the "Preferences" or "Settings" window, navigate to "Languages & Frameworks" > "Flutter."
- Set the Flutter SDK path to the location where Flutter is installed.

### 3. Install Flutter Dependencies:

- Open a terminal and run the command `flutter doctor` to check for any missing dependencies.
- Install any missing dependencies as suggested by the `flutter doctor` output.

### 4. Create a New Flutter Project:

- In Android Studio, go to "File" > "New" > "New Flutter Project."
- Select "Flutter Application" and click "Next."
- Enter the project name, choose a directory, and set other project options.
- Click "Finish" to create the project.

### 5. Open the Project:

- Once the project is created, open it by navigating to "File" > "Open" and selecting the project directory.

### 6. Install Android Virtual Device (AVD):

- Go to "Tools" > "AVD Manager" to open the Android Virtual Device Manager.
- Click "Create Virtual Device" to set up an Android emulator.
- Choose a hardware profile and system image, then click "Next" to configure the AVD.
- Complete the AVD creation process.

### 7. Run the Flutter App:

- Open the terminal in Android Studio.
- Navigate to the root directory of your Flutter project.
- Run the command `flutter run` to build and launch the app on the connected emulator.

### 8. Hot Reload:

- During development, use the hot reload feature by pressing `r` in the terminal to quickly see changes without restarting the app.

You've successfully set up Android Studio for Flutter development! Start building your Flutter project within Android Studio.

# Firebase Authentication Setup for Android Apps

Follow these steps to integrate Firebase Authentication with your Android app using Google Sign-In.

1. Click on "Add Project" and proceed with the instructions to establish a new project. Provide a name for your project and select your country or region.
2. After creating your project, click on "Add app" to include your app in the project. Choose the platform (iOS, Android, or Web) and follow the provided setup instructions.
3. For mobile apps, supply the package name (for Android) or bundle ID (for iOS).
4. Generate the SHA-1 key, enter it during the registration, and complete the registration process.
5. Upon registering your app, you'll receive a prompt to download a configuration file like `google-services.json` for Android. Place these files in the respective directories within your project.
6. For mobile apps, incorporate the necessary dependencies in your app-level `build.gradle` file.
7. Run your app and confirm the successful integration of Firebase. Check the console for logs indicating the successful initialization.
8. In the Firebase Console, navigate to "Authentication" and then to the "Sign-in method" tab. Enable the "Google" sign-in provider.
9. For Android, add the Firebase Authentication and Google Sign-In dependencies to your `build.gradle` file.
10. In your `MainActivity` or another appropriate activity, initiate Firebase Authentication. Set up Google Sign-In options. Create a `GoogleSignInClient` instance using the configured options.
11. Initiate the Google Sign-In process when the user clicks a button or takes a relevant action. Override the `onActivityResult` method to manage the outcome of the sign-in activity.
12. Implement the `handleSignInResult` method to handle and process the sign-in result. After acquiring the `GoogleSignInAccount`, proceed with the authentication through Firebase.
