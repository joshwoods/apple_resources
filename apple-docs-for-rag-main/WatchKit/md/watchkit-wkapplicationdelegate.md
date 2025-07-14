

- WatchKit
-  WKApplicationDelegate 

Protocol

# WKApplicationDelegate

A collection of methods that manages the app-level behavior for a single-target watchOS app.

watchOS 7.0+

``` source
@MainActor
protocol WKApplicationDelegate : NSObjectProtocol
```

## Mentioned in 

Using background tasks

## Overview

Implement the delegate’s methods to respond to your app’s life-cycle events, such as the activation and deactivation of your app. You can also implement delegate methods to respond to background tasks, Siri intents, workout sessions, or Handoff activity from another devices.

To add an app delegate, define a delegate class that subclasses NSObject and adopts the WKApplicationDelegate protocol.

```
import WatchKit

class MyWatchAppDelegate: NSObject, WKApplicationDelegate {

}
```

Then define an app delegate adaptor in your SwiftUI App structure.

```
import SwiftUI

@main
struct MyWatchApp_Watch_AppApp: App {
    @WKApplicationDelegateAdaptor var appDelegate: MyWatchAppDelegate
    var body: some Scene {
        WindowGroup {
            NavigationStack {
                ContentView()
            }
        }
    }
}

```

Finally, implement the delegate methods you want to handle.

## Topics

### Monitoring state changes

Working with the watchOS app life cycle

Learn how the watchOS app life cycle operates and responds to life cycle notification methods.

static func main()

Provides the top-level entry point for an app.

func applicationDidFinishLaunching()

Tells the delegate that the launch process is almost done and the app is almost ready to run.

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

### Handling extended runtime tasks

func handle(WKExtendedRuntimeSession)

Tells the delegate that the system launched your app to resume an extended runtime session.

### Managing remote notifications

func didRegisterForRemoteNotifications(withDeviceToken: Data)

Tells the delegate that the app successfully registered with Apple Push Notification service (APNs).

func didFailToRegisterForRemoteNotificationsWithError(any Error)

Tells the delegate that Apple Push Notification service (APNs) can’t successfully complete the registration process.

func didReceiveRemoteNotification([AnyHashable : Any], fetchCompletionHandler: (WKBackgroundFetchResult) -> Void)

Tells the delegate that a background notification has arrived.

enum WKBackgroundFetchResult

The result of an attempt to download the content associated with a remote notification.

### Coordinating Handoff activity

func handleUserActivity([AnyHashable : Any]?)

Responds to Handoff–related activity from complications and notifications.

func handle(NSUserActivity)

Responds to Handoff–related activity from Siri.

### Accepting CloudKit shares

func userDidAcceptCloudKitShare(with: CKShareMetadata)

Tells the delegate that the app has access to shared information in CloudKit.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### App structure

Setting up a watchOS project

Create a new watchOS project or add a watch target to an existing iOS project.

class WKApplication

The centralized point of control and coordination for apps with a single watchOS app target.

class WKExtension

The centralized point of control and coordination for extension-based apps running in watchOS.

protocol WKExtensionDelegate

A collection of methods that manages the app-level behavior of a WatchKit extension.

func WKApplicationMain(Int32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>, String?) -> Int32

Creates the application object and the application delegate, and sets up the app’s event cycle.

class WKInterfaceDevice

An object that provides information about the user’s Apple Watch.

WKPrefersNetworkUponForeground

A Boolean value that indicates whether an app requires network access on launch.

