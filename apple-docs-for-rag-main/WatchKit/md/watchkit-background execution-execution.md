

- WatchKit
-  Background execution 

API Collection

# Background execution

Manage background sessions and tasks.

## Overview

Apps on watchOS primarily run in the foreground to limit the impact on system resources. However, sometimes an app needs to perform an action when it’s not the foreground app. For a limited number of cases, watchOS provides options for running in the background.

### Handle background notifications

When the system launches your app in the background, you can:

- Handle background notifications from local or remote notifications with a UNUserNotificationCenterDelegate delegate. For more information, see Handling notifications and notification-related actions.

- Receive push notifications to update your app’s complications with a PKPushRegistryDelegate delegate. For more information, see PushKit.

### Schedule and handle background refresh tasks

A watchOS app uses a *background refresh task* to perform work in the background. If your app requires background operations, use one of the following techniques to respond to the task:

- Add a backgroundTask(_:action:) modifier to respond to the background task in your SwiftUI scene.

- Implement your app delegate’s handle(_:) method to receive and respond to the task. You need to call the task’s setTaskCompletedWithSnapshot(_:) method to indicate that you’re done.

In both cases, the system launches your app and gives it a few seconds of background execution time to perform the task. Complete the background task as quickly as possible. For more information, see Using background tasks.

### Start background sessions

Apps that support workouts, audio playback, or location updates can continue to run in the background until the current session ends. Your app must enable the appropriate background mode in your project’s capabilities, and then start the session while your app is running in the foreground.

- Use an HKWorkoutSession object to start and stop workouts. For more information, see Running workout sessions.

- Use the AVAudioSession class to play extended audio files in the background. For more information, see Playing Background Audio.

- Use a CLLocationManager object to start a continuous background location session. For more information, see allowsBackgroundLocationUpdates.

### Set up extended runtime sessions

Extended runtime sessions give your app additional time to run while the session is active. Extended runtime sessions provide support for the following session types:

- Self care

- Mindfulness

- Physical therapy

- Smart alarm

Extended runtime sessions let the app continue to communicate with a Bluetooth device, process data, or play sounds or haptics, even after the watch’s screen turns off. While most extended runtime sessions run your app as the frontmost app, some sessions run your app in the background. Select a session type based on the app’s intended use — not based on the features that the session provides.

For more information, see Using extended runtime sessions.

## Topics

### Background tasks

Using background tasks

Handle scheduled update tasks in the background, and respond to background system interactions including Siri intents and incoming Bluetooth messages.

Preparing to take your watchOS app’s snapshot

Provide a timely, accurate snapshot of your app by using snapshot background tasks.

class WKApplicationRefreshBackgroundTask

A task that updates your app’s state in the background.

class WKURLSessionRefreshBackgroundTask

A task that responds to background URL sessions.

class WKWatchConnectivityRefreshBackgroundTask

A background task used to receive background updates from the Watch Connectivity framework.

class WKBluetoothAlertRefreshBackgroundTask

A task for handling timely Bluetooth alerts in the background.

class WKIntentDidRunRefreshBackgroundTask

A background task used to update your app after a SiriKit intent runs.

class WKRelevantShortcutRefreshBackgroundTask

A background task used to periodically donate relevant Siri shortcuts.

class WKSnapshotRefreshBackgroundTask

A background task used to update your app’s user interface in preparation for a snapshot.

class WKRefreshBackgroundTask

The abstract superclass for WatchKit’s background task classes.

### Background sessions

Enabling Background Sessions

Enable the background mode for audio, location updates, remote notifications, or workouts.

Playing Background Audio

Enable background audio in your app to provide a seamless playback experience.

WKBackgroundModes

The services a watchOS app provides that require it to continue running in the background.

UIBackgroundModes

Services provided by an app that require it to run in the background.

## See Also

### Runtime management

Life cycles

Receive and respond to life-cycle notifications.

Using extended runtime sessions

Create an extended runtime session that continues running your app after the user stops interacting with it.

class WKExtendedRuntimeSession

A session that continues to run your app after the user has stopped interacting.

Interacting with Bluetooth peripherals during background app refresh

Keep your complications up-to-date by reading values from a Bluetooth peripheral while your app is running in the background.

