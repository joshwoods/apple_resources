

- WatchKit
- Background execution
-  Enabling Background Sessions 

Article

# Enabling Background Sessions

Enable the background mode for audio, location updates, remote notifications, or workouts.

## Overview

To receive background notifications or run background sessions, your app needs to enable the corresponding background mode. Add the Background Modes capability to your WatchKit extension, and then select the desired modes. Each mode sets its respective keys in the extension’s `Info.plist` file.

The Remote notification mode lets your app receive remote, background notifications. When a background notification arrives, the system wakes or launches your app to the background and gives it 30 seconds to update the app. For more information, see Pushing background updates to your App.

The Audio, Location updates, and Workout processing modes let your app run the respective background sessions. Your app must start the session in the foreground, but the session continues to run when your app transitions to the background. Also, while the session is running, Apple Watch displays your app whenever the user raises their wrist. If the user presses the digital crown to navigate back to the watch face, the system displays an icon above the status bar, indicating that the session is still active.

- Use an HKWorkoutSession object to start and stop workouts. For more information, see Running workout sessions.

- Use the AVAudioSession class to play extended audio files in the background. For more information see Playing Background Audio.

- Use a CLLocationManager object to start a continuous background location session. For more information, see allowsBackgroundLocationUpdates.

## See Also

### Background sessions

Playing Background Audio

Enable background audio in your app to provide a seamless playback experience.

WKBackgroundModes

The services a watchOS app provides that require it to continue running in the background.

UIBackgroundModes

Services provided by an app that require it to run in the background.

