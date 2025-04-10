# UAC Companion

This Flutter app serves as a companion app for the "Ultimate Alarm Clock by CCExtractor Development".

Demo Video: [Watch on YouTube](https://youtu.be/T0aBws2LN2o)

## Getting Started
To use this companion app, you’ll need to run both of the following repositories simultaneously:

[flutter_uac_companion](https://github.com/Abhishek14104/flutter_uac_companion) – this Wear OS companion app.

[ultimate_alarm_clock](https://github.com/Abhishek14104/ultimate_alarm_clock/tree/flutter_companion) (flutter_companion branch) – the main UAC app that runs on your Android phone.


## Major Technologies

- [Wearable Data Layer API](https://developer.android.com/training/wearables/data/overview) - Provides a communication channel between wearable devices.
- [MethodChannels](https://docs.flutter.dev/platform-integration/platform-channels) - Helps to use platform-specific code in your Flutter app.
- [EventChannels](https://api.flutter.dev/flutter/services/EventChannel-class.html#:~:text=A%20named%20channel%20for%20communicating,are%20decoded%20into%20Dart%20values.) - A named channel for communicating with platform plugins using event streams.

## Permissions Given

- [android.permission.WAKE_LOCK](https://developer.android.com/develop/background-work/background-tasks/awake/wakelock)

## Steps to Run Locally


1. Clone the Repositories
   ```bash
   git clone https://github.com/Abhishek14104/flutter_uac_companion.git
   git clone -b flutter_companion https://github.com/Abhishek14104/ultimate_alarm_clock.git
   ```

2. Navigate to the Project Directories
   ```bash
   cd flutter_uac_companion
   ```

   And in a separate terminal:
   ```bash
   cd ultimate_alarm_clock
   ```
3. **Install Dependencies**: Install the required dependencies by running:
In both terminals:
   ```bash
   flutter pub get
   ```

4. **Run the Application**: Launch the app on any WearOS (for uac_companion)/Android (for UAC) devices:

   ```bash
   flutter run
   ```
