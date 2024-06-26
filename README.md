## TODO
- Enable VM acceleration on your development computer.

# FlutterApp
This repo contains guides on installing Flutter and the development of an Android App. 

# Installation 
- Install Flutter (I used Windows and Android since this is recommended for Windows)
  - This requires Git for Windows
- This also requires Android Studio (2023.2.1) or later to compile and debug Java and Kotlin code. (ARM CPUs are not supported!!) (https://developer.android.com/studio/install#windows) 
  - https://developer.android.com/studio?_gl=1*1l5giai*_up*MQ..&gclid=CjwKCAjwrcKxBhBMEiwAIVF8rL8-ZuXj8PXxP9IEfy_iwru8xFp7afqxQ1MxfDrupGRvKWWlwbM_xhoCZkAQAvD_BwE&gclsrc=aw.ds
- Install an IDE capable of code completion, syntax highlighting, and more features.
  - Visual Studio Code is recommended
 
# Installing the Flutter SDK
- Download the flutter zip file from "Download and install" https://docs.flutter.dev/get-started/install/windows/mobile?tab=download
- run the following command in PowerShell
  Expand-Archive -Path $env:USERPROFILE\Downloads\flutter_windows_3.19.6-stable.zip -Destination $env:USERPROFILE\dev\
- Open System>Advanced System Setting> Advanced> Environment Variables
- In the User variables for (username) section, look for the Path entry.
    If the entry exists, double-click on it.
    The Edit Environment Variable dialog displays.
    Double-click in an empty row.
    Type %USERPROFILE%\dev\flutter\bin.
    Click the %USERPROFILE%\dev\flutter\bin entry.
    Click Move Up until the Flutter entry sits at the top of the list.
    Click OK three times.
- To enable these changes, close and reopen any existing command prompts and PowerShell instances.

# Configure Android Development
- To create Android apps with Flutter, verify that the following Android components have been installed.

Android SDK Platform, API 34.0.0
Android SDK Command-line Tools
Android SDK Build-Tools
Android SDK Platform-Tools
Android Emulator

# Configure your target Android device
- press on 'more actions'
- click on device and run

# Agree to Android Licenses
- Open powershell and run
  flutter doctor --android-licenses

# Check your development setup
- In powershell, run:
  flutter doctor

## Bugs I encountered
- Android toolchain cmdline-tools missing
- Solution
- - https://stackoverflow.com/questions/60475481/flutter-doctor-error-android-sdkmanager-tool-not-found-windows
 
# Test Drive 
- To run your first app, launch Android Studio.
- Click 'new'
- Click 'empty'
- Enter 'test drive' into the name and press 'create'
- Add a configuration for 'test_drive'
- Run and apply live edits to begin 
  
