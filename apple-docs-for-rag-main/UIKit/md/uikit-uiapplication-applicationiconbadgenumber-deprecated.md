

- UIKit
- UIApplication
-  applicationIconBadgeNumber Deprecated

Instance Property

# applicationIconBadgeNumber

The number currently set as the badge of the app icon on the Home screen.

iOS 2.0–17.0DeprecatediPadOS 2.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var applicationIconBadgeNumber: Int { get set }
```

Deprecated

Use setBadgeCount(_:withCompletionHandler:) instead.

## Discussion

Set to 0 (zero) to hide the badge number. The default value of this property is 0.

## See Also

### Deprecated properties

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

