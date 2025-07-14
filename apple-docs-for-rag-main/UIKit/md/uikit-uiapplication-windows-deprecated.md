

- UIKit
- UIApplication
-  windows Deprecated

Instance Property

# windows

The app’s visible and hidden windows.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var windows: [UIWindow] { get }
```

Deprecated

Use the windows property of the relevant window scene.

## Discussion

This property contains the UIWindow objects currently associated with the app. This list doesn’t include windows created and managed by the system, such as the window used to display the status bar.

The array orders the windows from back to front by window level; thus, the last window in the array is on top of all other app windows.

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

