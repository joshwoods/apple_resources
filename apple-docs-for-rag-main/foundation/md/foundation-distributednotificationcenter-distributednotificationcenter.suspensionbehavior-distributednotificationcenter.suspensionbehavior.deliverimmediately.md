

- Foundation
- DistributedNotificationCenter
- DistributedNotificationCenter.SuspensionBehavior
-  DistributedNotificationCenter.SuspensionBehavior.deliverImmediately 

Case

# DistributedNotificationCenter.SuspensionBehavior.deliverImmediately

Mac Catalyst 13.0+macOS 10.0+

``` source
case deliverImmediately
```

## Discussion

The server delivers notifications matching this registration irrespective of whether suspended with an argument of true has been called. When a notification with this suspension behavior is matched, it has the effect of first flushing any queued notifications. The effect is as if suspended with an argument of false were first called if the application is suspended, followed by the notification in question being delivered, followed by a transition back to the previous suspended or unsuspended state.

## See Also

### Constants

case drop

The server does not queue any notifications with this name and object until suspended with an argument of false is called.

case coalesce

The server only queues the last notification of the specified name and object; earlier notifications are dropped. In cover methods for which suspension behavior is not an explicit argument, `NSNotificationSuspensionBehaviorCoalesce` is the default.

case hold

The server holds all matching notifications until the queue has been filled (queue size determined by the server), at which point the server may flush queued notifications.

case drop

The server does not queue any notifications with this name and object until suspended with an argument of false is called.

case coalesce

The server only queues the last notification of the specified name and object; earlier notifications are dropped. In cover methods for which suspension behavior is not an explicit argument, `NSNotificationSuspensionBehaviorCoalesce` is the default.

case hold

The server holds all matching notifications until the queue has been filled (queue size determined by the server), at which point the server may flush queued notifications.

