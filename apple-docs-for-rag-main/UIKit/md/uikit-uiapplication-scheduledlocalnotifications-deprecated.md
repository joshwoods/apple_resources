

- UIKit
- UIApplication
-  scheduledLocalNotifications Deprecated

Instance Property

# scheduledLocalNotifications

All currently scheduled local notifications.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var scheduledLocalNotifications: [UILocalNotification]? { get set }
```

Deprecated

Use the UNUserNotificationCenter class to schedule local notifications instead.

## Discussion

This property holds an array of UILocalNotification objects representing the current scheduled local notifications. Use this property to access the currently scheduled notifications, perhaps to cancel them. Assigning a new value to this property implicitly schedules all of the notifications in the new array.

This method may be faster than using scheduleLocalNotification(_:) when scheduling a large number of notifications.

## See Also

### Deprecated properties

var applicationIconBadgeNumber: Int

The number currently set as the badge of the app icon on the Home screen.

Deprecated

class let statusBarFrameUserInfoKey: String

A key whose value indicates the new status bar frame.

Deprecated

class let statusBarOrientationUserInfoKey: String

A key whose value indicates the current interface orientation.

Deprecated

var currentUserNotificationSettings: UIUserNotificationSettings?

Returns the user notification settings for the app.

Deprecated

var isIgnoringInteractionEvents: Bool

A Boolean value that indicates whether the receiver is ignoring events initiated by touches on the screen.

Deprecated

var isNetworkActivityIndicatorVisible: Bool

A Boolean value that turns an indicator of network activity on or off.

Deprecated

var isStatusBarHidden: Bool

A Boolean value that determines whether the status bar is hidden.

Deprecated

var keyWindow: UIWindow?

The app’s key window.

Deprecated

var statusBarFrame: CGRect

The frame rectangle defining the area of the status bar.

Deprecated

var statusBarOrientation: UIInterfaceOrientation

The current orientation of the app’s status bar.

Deprecated

var statusBarOrientationAnimationDuration: TimeInterval

The animation duration in seconds for the status bar during a 90 degree orientation change.

Deprecated

var statusBarStyle: UIStatusBarStyle

The current style of the status bar.

Deprecated

var windows: [UIWindow]

The app’s visible and hidden windows.

Deprecated

