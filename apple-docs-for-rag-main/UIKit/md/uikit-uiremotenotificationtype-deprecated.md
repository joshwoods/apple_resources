

- UIKit
-  UIRemoteNotificationType Deprecated

Structure

# UIRemoteNotificationType

Constants indicating the types of notifications the app may display to the user.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
struct UIRemoteNotificationType
```

## Overview

One or more of the values in the `UIRemoteNotificationType` bit mask are passed to iOS as the argument of the registerForRemoteNotifications(matching:) method. Thereafter, iOS filters notifications for the app based on these values. You can always get the current notification types by calling the enabledRemoteNotificationTypes() method.

## Topics

### Constants

static var badge: UIRemoteNotificationType

The app accepts notifications that badge the app icon.

static var sound: UIRemoteNotificationType

The app accepts alert sounds as notifications.

static var alert: UIRemoteNotificationType

The app accepts alert messages as notifications.

static var newsstandContentAvailability: UIRemoteNotificationType

The app accepts notifications that start the downloading of issue assets for Newsstand apps.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Deprecated methods

func requestSceneSessionActivation(UISceneSession?, userActivity: NSUserActivity?, options: UIScene.ActivationRequestOptions?, errorHandler: ((any Error) -> Void)?)

Asks the system to activate an existing scene, or create a new scene and associate it with your app.

Deprecated

func beginIgnoringInteractionEvents()

Tells the receiver to suspend the handling of touch-related events.

Deprecated

func endIgnoringInteractionEvents()

Tells the receiver to resume the handling of touch-related events.

Deprecated

func setMinimumBackgroundFetchInterval(TimeInterval)

Specifies the minimum amount of time that must elapse between background fetch operations.

Deprecated

func scheduleLocalNotification(UILocalNotification)

Schedules a local notification for delivery at its encapsulated date and time.

Deprecated

func presentLocalNotificationNow(UILocalNotification)

Presents a local notification immediately.

Deprecated

func cancelLocalNotification(UILocalNotification)

Cancels the delivery of the specified scheduled local notification.

Deprecated

func cancelAllLocalNotifications()

Cancels the delivery of all scheduled local notifications.

Deprecated

func setKeepAliveTimeout(TimeInterval, handler: (() -> Void)?) -> Bool

Configures a periodic handler for VoIP apps in older versions of iOS.

Deprecated

let UIMinimumKeepAliveTimeout: TimeInterval

The minimum amount of time (measured in seconds) an app may run a critical background task in the background.

Deprecated

func clearKeepAliveTimeout()

Removes a previously installed periodic handler block.

Deprecated

func setStatusBarHidden(Bool, with: UIStatusBarAnimation)

Hides or shows the status bar, optionally animating the transition.

Deprecated

func setStatusBarStyle(UIStatusBarStyle, animated: Bool)

Sets the style of the status bar, optionally animating the transition to the new style.

Deprecated

func setStatusBarOrientation(UIInterfaceOrientation, animated: Bool)

Sets the app’s status bar to the specified orientation, optionally animating the transition.

Deprecated

func registerUserNotificationSettings(UIUserNotificationSettings)

Registers your preferred options for notifying the user.

Deprecated

