

- UIKit
- UIApplication
-  keyWindow Deprecated

Instance Property

# keyWindow

The app’s key window.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
var keyWindow: UIWindow? { get }
```

## Discussion

This property holds the UIWindow object in the windows array that is most recently sent the makeKeyAndVisible() message.

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

