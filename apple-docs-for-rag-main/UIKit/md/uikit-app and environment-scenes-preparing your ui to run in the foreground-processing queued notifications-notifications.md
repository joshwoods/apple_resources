

- UIKit
- App and environment
- Scenes
- Preparing your UI to run in the foreground
-  Processing queued notifications 

Article

# Processing queued notifications

Respond to notifications when coming out of the suspended state.

## Overview

When settings or device conditions change, the system generates notifications so that apps can respond accordingly. These notifications are delivered immediately to apps that are running, but their delivery is delayed for apps that are suspended. For a suspended app, pending notifications are delivered as soon after the app begins running again (either in the foreground or in the background).

The following table lists the notifications that apps can receive after they start running again. You must explicitly add an observer to these notifications to receive them. The system coalesces multiple related notifications so that the app receives only one notification with the net changes.

| Event | Notifications |
|----|----|
| The user changed your app’s preferences | didChangeNotification |
| The current language or locale settings changed | currentLocaleDidChangeNotification |
| The screen mode of a display changes | modeDidChangeNotification |
| An external display is connected or disconnected | didConnectNotification  didDisconnectNotification |
| An accessory is connected or disconnected | EAAccessoryDidConnect (Swift) or EAAccessoryDidConnectNotification (Objective-C)  EAAccessoryDidDisconnect (Swift) or EAAccessoryDidDisconnectNotification (Objective-C) |
| The status of the user’s iCloud account changed | NSUbiquityIdentityDidChange |
| The device orientation changed | orientationDidChangeNotification  (UIKit automatically updates the interface orientation of your view controllers when appropriate.) |
| There was a significant time change | significantTimeChangeNotification |
| The battery level or battery state changed | batteryLevelDidChangeNotification  batteryStateDidChangeNotification |
| The device’s proximity to the user changed | proximityStateDidChangeNotification |

When a suspended app starts running again, the system delivers any queued notifications on the app’s main thread before it delivers any touch events or user input. Handle all notifications as quickly as possible.

