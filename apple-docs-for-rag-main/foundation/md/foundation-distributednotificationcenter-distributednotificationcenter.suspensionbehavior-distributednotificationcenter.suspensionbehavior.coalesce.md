

- Foundation
- DistributedNotificationCenter
- DistributedNotificationCenter.SuspensionBehavior
-  DistributedNotificationCenter.SuspensionBehavior.coalesce 

Case

# DistributedNotificationCenter.SuspensionBehavior.coalesce

The server only queues the last notification of the specified name and object; earlier notifications are dropped. In cover methods for which suspension behavior is not an explicit argument, `NSNotificationSuspensionBehaviorCoalesce` is the default.

Mac Catalyst 13.0+macOS 10.0+

``` source
case coalesce
```

## See Also

### Constants

case drop

The server does not queue any notifications with this name and object until suspended with an argument of false is called.

case hold

The server holds all matching notifications until the queue has been filled (queue size determined by the server), at which point the server may flush queued notifications.

case deliverImmediately

case drop

The server does not queue any notifications with this name and object until suspended with an argument of false is called.

case hold

The server holds all matching notifications until the queue has been filled (queue size determined by the server), at which point the server may flush queued notifications.

case deliverImmediately

