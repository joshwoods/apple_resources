

- UIKit
- UIApplication
-  currentUserNotificationSettings Deprecated

Instance Property

# currentUserNotificationSettings

Returns the user notification settings for the app.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var currentUserNotificationSettings: UIUserNotificationSettings? { get }
```

Deprecated

Use UNUserNotificationCenter instead.

## Return Value

A user notification settings object indicating the types of notifications that your app may use.

## Discussion

If you configure local or remote notifications with unavailable notification types, the system does not display the corresponding alerts to the user. The system does still deliver the local and remote notifications to your app.

## See Also

### Related Documentation

func registerUserNotificationSettings(UIUserNotificationSettings)

Registers your preferred options for notifying the user.

Deprecated

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

var scheduledLocalNotifications: [UILocalNotification]?

All currently scheduled local notifications.

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

