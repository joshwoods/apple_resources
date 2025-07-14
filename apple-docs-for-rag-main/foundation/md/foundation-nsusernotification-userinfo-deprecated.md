

- Foundation
- NSUserNotification
-  userInfo Deprecated

Instance Property

# userInfo

Application-specific user info that can be attached to the notification.

macOS 10.8–11.0Deprecated

``` source
var userInfo: [String : Any]? { get set }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

All items must be property list types or an exception is thrown.

The `userInfo` content must be of reasonable serialized size (less than 1KB) or an exception is thrown.

