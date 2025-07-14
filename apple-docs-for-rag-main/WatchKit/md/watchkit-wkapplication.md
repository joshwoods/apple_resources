

- WatchKit
-  WKApplication 

Class

# WKApplication

The centralized point of control and coordination for apps with a single watchOS app target.

watchOS 7.0+

``` source
@MainActor
class WKApplication
```

## Overview

In Xcode 13 and earlier, the system divides a watchOS app into two sections:

WatchKit app  
An app bundle that contains your app icon. For storyboard-based apps, it also includes your storyboard and any assets used by the storyboard.

WatchKit extension  
An extension that contains your watchOS app’s code.

In Xcode 14 and later, you can produce watchOS apps with a single watchOS app target for code, assets, extensions, and localizations. These single-target watchOS apps can run on watchOS 7 and later

Single-target watchOS apps have a single app object. While the system creates and manages this object, you can access it to perform app-level tasks such as opening URLs and getting the root interface controller of your app.

As relevant events occur within your WatchKit app, the app object notifies its delegate of those events. Your delegate object can implement the methods it needs to provide an appropriate response to life-cycle events, handle notifications, or handle Handoff–related behaviors. For more information about the methods of the delegate, see WKApplicationDelegate.

## Topics

### Getting the app object

class func shared() -> WKApplication

Returns the shared WatchKit app object.

### Accessing the app delegate

var delegate: (any WKApplicationDelegate)?

The delegate of the WatchKit app object.

protocol WKApplicationDelegate

A collection of methods that manages the app-level behavior for a single-target watchOS app.

### Opening a URL resource

func openSystemURL(URL)

Opens the specified system URL.

### Getting the interface controller

var rootInterfaceController: WKInterfaceController?

The app’s root interface controller.

var visibleInterfaceController: WKInterfaceController?

Returns the last visible interface controller.

### Managing the app state

var applicationState: WKApplicationState

The runtime state of the watchOS app.

enum WKApplicationState

The running states of the Watch app.

var isApplicationRunningInDock: Bool

A Boolean value that indicates whether the app is running in the dock.

func scheduleBackgroundRefresh(withPreferredDate: Date, userInfo: (any NSSecureCoding &amp; NSObjectProtocol)?, scheduledCompletion: ((any Error)?) -> Void)

Schedules a background task to refresh the app’s data.

### Managing the user interface

var isAutorotating: Bool

A Boolean value that determines whether the interface automatically rotates when the user flips their wrist.

var isAutorotated: Bool

A Boolean value that indicates whether the system has automatically rotated the user interface, orienting it properly for another viewer.

var globalTintColor: UIColor

The watchOS app’s global tint color.

### Managing the snapshot

func scheduleSnapshotRefresh(withPreferredDate: Date, userInfo: (any NSSecureCoding &amp; NSObjectProtocol)?, scheduledCompletion: ((any Error)?) -> Void)

Schedules a background task to refresh your app’s snapshot.

### Observing messages from the notification center

static let didFinishLaunchingNotification: NSNotification.Name

A message indicating that the launch process finished and the extension is ready to run.

static let didBecomeActiveNotification: NSNotification.Name

A message indicating that the watchOS app is visible and processing events.

static let willResignActiveNotification: NSNotification.Name

A message indicating that the system is about to deactivate the watchOS app.

static let willEnterForegroundNotification: NSNotification.Name

A message indicating that the watchOS app is about to transition from the background to the foreground.

static let didEnterBackgroundNotification: NSNotification.Name

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

protocol WKApplicationDelegate

A collection of methods that manages the app-level behavior for a single-target watchOS app.

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

