

- Foundation
- NSUserNotification
-  NSUserNotification.ActivationType Deprecated

Enumeration

# NSUserNotification.ActivationType

These constants describe how the user notification was activated.

macOS 10.8–11.0Deprecated

``` source
enum ActivationType
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Topics

### Constants

case none

The user did not interact with the notification alert.

case contentsClicked

The user clicked on the contents of the notification alert.

case actionButtonClicked

The user clicked on the action button of the notification alert.

case replied

The user replied to the notification.

case additionalActionClicked

The user clicked on the additional action button of the notification alert.

case none

The user did not interact with the notification alert.

case contentsClicked

The user clicked on the contents of the notification alert.

case actionButtonClicked

The user clicked on the action button of the notification alert.

case replied

The user replied to the notification.

case additionalActionClicked

The user clicked on the additional action button of the notification alert.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

let NSUserNotificationDefaultSoundName: String

The default notification sound.

Deprecated

