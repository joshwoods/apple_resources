

- Foundation
- NSUserNotificationCenter
-  delegate Deprecated

Instance Property

# delegate

Specifies the notification center delegate.

macOS 10.8–11.0Deprecated

``` source
unowned(unsafe) var delegate: (any NSUserNotificationCenterDelegate)? { get set }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

The delegate must conform to the NSUserNotificationCenterDelegate protocol.

