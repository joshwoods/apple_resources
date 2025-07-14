

- Core Foundation
-  CFNotificationSuspensionBehavior 

Enumeration

# CFNotificationSuspensionBehavior

Suspension flags that indicate how distributed notifications should be handled when the receiving application is in the background.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFNotificationSuspensionBehavior
```

## Overview

An application selects the suspension behavior for a given notification when it registers an observer for that notification with CFNotificationCenterAddObserver(_:_:_:_:_:_:).

## Topics

### Constants

case drop

The server will not queue any notifications of the specified name and object while the receiving application is in the background.

case coalesce

The server will only queue the last notification of the specified name and object; earlier notifications are dropped.

case hold

The server will hold all matching notifications until the queue has been filled (queue size determined by the server) at which point the server may flush queued notifications.

case deliverImmediately

The server will deliver notifications of the specified name and object whether or not the application is in the background. When a notification with this suspension behavior is matched, it has the effect of first flushing any queued notifications.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

Notification Posting Options

Possible options when posting notifications.

