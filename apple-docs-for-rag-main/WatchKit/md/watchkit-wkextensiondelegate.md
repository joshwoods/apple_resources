

- WatchKit
-  WKExtensionDelegate 

Protocol

# WKExtensionDelegate

A collection of methods that manages the app-level behavior of a WatchKit extension.

watchOS 2.0+

``` source
@MainActor
protocol WKExtensionDelegate : NSObjectProtocol
```

## Overview

Implement the delegate’s methods to respond to your app’s life-cycle events, such as the activation and deactivation of your app. You can also implement delegate methods to respond to background tasks, Siri intents, workout sessions, or Handoff activity from another devices.

WatchKit creates your delegate object automatically by instantiating the class assigned to the WKExtensionDelegateClassName key in your WatchKit extension’s `Info.plist` file. By default, this class is named ExtensionDelegate. The system then assigns the delegate object to the delegate property of the shared WKExtension object.

## Topics

### Monitoring state changes

Working with the watchOS app life cycle

Learn how the watchOS app life cycle operates and responds to life cycle notification methods.

func applicationDidFinishLaunching()

Tells the delegate that the launch process is almost done and the extension is almost ready to run.

func applicationDidBecomeActive()

Tells the delegate that the watchOS app is visible and processing events.

func applicationWillResignActive()

Tells the delegate that the system is about to deactivate the watchOS app.

func applicationWillEnterForeground()

Tells the delegate that the app is about to transition from the background to the foreground.

func applicationDidEnterBackground()

Tells the delegate that the app has transitioned from the foreground to the background.

func deviceOrientationDidChange()

Tells the delegate that the device’s orientation has changed.

### Responding to intents

func handle(INIntent, completionHandler: (INIntentResponse) -> Void)

Responds to a Siri intent.

### Setup Now Playing interface

func handleRemoteNowPlayingActivity()

Tells the delegate when the user plays audio in the corresponding iOS app.

### Handling a workout session

func handle(HKWorkoutConfiguration)

Tells the delegate that the user started a workout session on the paired iPhone.

func handleActiveWorkoutRecovery()

Tells the delegate when the app relaunches after crashing during an active workout session.

### Handling background tasks

func handle(Set&lt;WKRefreshBackgroundTask>)

Tells the delegate that the app has received one or more background tasks.

### Handling extended runtime sessions

func handle(WKExtendedRuntimeSession)

Tells the delegate that the system launched your app to resume an extended runtime session.

### Managing remote notifications

func didRegisterForRemoteNotifications(withDeviceToken: Data)

Tells the delegate that the app successfully registered with Apple Push Notification service (APNs).

func didFailToRegisterForRemoteNotificationsWithError(any Error)

Tells the delegate that Apple Push Notification service (APNs) cannot successfully complete the registration process.

func didReceiveRemoteNotification([AnyHashable : Any], fetchCompletionHandler: (WKBackgroundFetchResult) -> Void)

Tells the delegate that a background notification has arrived.

enum WKBackgroundFetchResult

The result of an attempt to download the content associated with a remote notification.

### Coordinating handoff activity

func handleUserActivity([AnyHashable : Any]?)

Responds to Handoff–related activity from complications and notifications.

func handle(NSUserActivity)

Responds to Handoff–related activity from Siri.

### Accepting CloudKit shares

func userDidAcceptCloudKitShare(with: CKShareMetadata)

Tells the delegate that the app has access to shared information in CloudKit.

### Deprecated Methods

func didReceiveRemoteNotification([AnyHashable : Any])

Tells the delegate that a remote notification arrived.

Deprecated

func didReceive(UILocalNotification)

Tells the delegate that a local notification was triggered.

Deprecated

func handleAction(withIdentifier: String?, forRemoteNotification: [AnyHashable : Any])

Delivers a remote notification payload and a user-selected action to the app.

Deprecated

func handleAction(withIdentifier: String?, forRemoteNotification: [AnyHashable : Any], withResponseInfo: [AnyHashable : Any])

Delivers a remote notification payload and user response information to the app.

Deprecated

func handleAction(withIdentifier: String?, for: UILocalNotification)

Delivers a local notification payload and a user-selected action to the app.

Deprecated

func handleAction(withIdentifier: String?, for: UILocalNotification, withResponseInfo: [AnyHashable : Any])

Delivers a local notification payload and user response information to the app.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### App structure

Setting up a watchOS project

Create a new watchOS project or add a watch target to an existing iOS project.

class WKApplication

The centralized point of control and coordination for apps with a single watchOS app target.

protocol WKApplicationDelegate

A collection of methods that manages the app-level behavior for a single-target watchOS app.

class WKExtension

The centralized point of control and coordination for extension-based apps running in watchOS.

func WKApplicationMain(Int32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>, String?) -> Int32

Creates the application object and the application delegate, and sets up the app’s event cycle.

class WKInterfaceDevice

An object that provides information about the user’s Apple Watch.

WKPrefersNetworkUponForeground

A Boolean value that indicates whether an app requires network access on launch.

