

- WatchKit
-  WKExtension 

Class

# WKExtension

The centralized point of control and coordination for extension-based apps running in watchOS.

watchOS 2.0+

``` source
@MainActor
class WKExtension
```

## Overview

In Xcode 13 and earlier the system divides a watchOS app into two sections:

WatchKit app  
An app bundle that contains your app icon. For storyboard-based apps, it also includes your storyboard and any assets used by the storyboard.

WatchKit extension  
An extension that contains your watchOS app’s code.

In Xcode 14 and later, you can produce watchOS apps with a single watchOS app target for code, assets, extensions, and localizations. These single-target watchOS apps can run on watchOS 7 and later

Apps with separate WatchKit app and extensions have a single extension object. While the system creates and manages this object, you can access it to perform app-level tasks such as opening URLs and getting the root interface controller of your app.

As relevant events occur within your WatchKit app, the extension object notifies its delegate of those events. Your delegate object can implement the methods it needs to provide an appropriate response to life cycle events, handle notifications, or handle Handoff–related behaviors. For more information about the methods of the delegate, see WKExtensionDelegate.

## Topics

### Getting the extension object

class func shared() -> WKExtension

Returns the shared WatchKit extension object.

### Accessing the extension delegate

var delegate: (any WKExtensionDelegate)?

The delegate of the WatchKit extension object.

protocol WKExtensionDelegate

A collection of methods that manages the app-level behavior of a WatchKit extension.

### Opening a URL resource

func openSystemURL(URL)

Opens the specified system URL.

### Getting the interface controllers

var rootInterfaceController: WKInterfaceController?

The app’s root interface controller.

var visibleInterfaceController: WKInterfaceController?

Returns the last visible interface controller.

### Managing the execution state

var applicationState: WKApplicationState

The runtime state of the Watch app.

enum WKApplicationState

The running states of the Watch app.

var isApplicationRunningInDock: Bool

A Boolean value that indicates whether the app is running in the dock.

func scheduleBackgroundRefresh(withPreferredDate: Date, userInfo: (any NSSecureCoding &amp; NSObjectProtocol)?, scheduledCompletion: ((any Error)?) -> Void)

Schedules a background task to refresh the app’s data.

var isFrontmostTimeoutExtended: Bool

A Boolean value that determines whether the app extends its time as the frontmost app.

Deprecated

### Managing the user interface

var isAutorotating: Bool

A Boolean value that determines whether the interface automatically rotates when the user flips their wrist.

var isAutorotated: Bool

A Boolean value that indicates whether the system has automatically rotated the user interface so that it is properly oriented for another viewer.

var globalTintColor: UIColor

The watchOS app’s global tint color.

func enableWaterLock()

Disables the Apple Watch touch screen to prevent accidental taps while the watch is underwater.

Deprecated

### Managing the snapshot

func scheduleSnapshotRefresh(withPreferredDate: Date, userInfo: (any NSSecureCoding &amp; NSObjectProtocol)?, scheduledCompletion: ((any Error)?) -> Void)

Schedules a background task to refresh your app’s snapshot.

### Observing messages from the notification center

class let applicationDidFinishLaunchingNotification: NSNotification.Name

A message indicating that the launch process finished and the extension is ready to run.

class let applicationDidBecomeActiveNotification: NSNotification.Name

A message indicating that the watchOS app is visible and processing events.

class let applicationWillResignActiveNotification: NSNotification.Name

A message indicating that the system is about to deactivate the watchOS app.

class let applicationWillEnterForegroundNotification: NSNotification.Name

A message indicating that the watchOS app is about to transition from the background to the foreground.

class let applicationDidEnterBackgroundNotification: NSNotification.Name

A message indicating that the watchOS app transitioned from the foreground to the background.

### Registering for remote notifications

func registerForRemoteNotifications()

Register to receive remote notifications from the Apple Push Notification service (APNs).

func unregisterForRemoteNotifications()

Unregister for all remote notifications received from Apple Push Notification service (APNs).

var isRegisteredForRemoteNotifications: Bool

A Boolean value that indicates if the app has successfully registered for remote notifications.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### App structure

Setting up a watchOS project

Create a new watchOS project or add a watch target to an existing iOS project.

class WKApplication

The centralized point of control and coordination for apps with a single watchOS app target.

protocol WKApplicationDelegate

A collection of methods that manages the app-level behavior for a single-target watchOS app.

protocol WKExtensionDelegate

A collection of methods that manages the app-level behavior of a WatchKit extension.

func WKApplicationMain(Int32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;CChar>?>, String?) -> Int32

Creates the application object and the application delegate, and sets up the app’s event cycle.

class WKInterfaceDevice

An object that provides information about the user’s Apple Watch.

WKPrefersNetworkUponForeground

A Boolean value that indicates whether an app requires network access on launch.

