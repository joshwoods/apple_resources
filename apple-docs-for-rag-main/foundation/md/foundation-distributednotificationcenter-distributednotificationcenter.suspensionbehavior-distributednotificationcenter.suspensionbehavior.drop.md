

- Foundation
- DistributedNotificationCenter
- DistributedNotificationCenter.SuspensionBehavior
-  DistributedNotificationCenter.SuspensionBehavior.drop 

Case

# DistributedNotificationCenter.SuspensionBehavior.drop

The server does not queue any notifications with this name and object until suspended with an argument of false is called.

Mac Catalyst 13.0+macOS 10.0+

``` source
case drop
```

## See Also

### Constants

case coalesce

The server only queues the last notification of the specified name and object; earlier notifications are dropped. In cover methods for which suspension behavior is not an explicit argument, `NSNotificationSuspensionBehaviorCoalesce` is the default.

case hold

The server holds all matching notifications until the queue has been filled (queue size determined by the server), at which point the server may flush queued notifications.

case deliverImmediately

case coalesce

The server only queues the last notification of the specified name and object; earlier notifications are dropped. In cover methods for which suspension behavior is not an explicit argument, `NSNotificationSuspensionBehaviorCoalesce` is the default.

case hold

The server holds all matching notifications until the queue has been filled (queue size determined by the server), at which point the server may flush queued notifications.

case deliverImmediately

