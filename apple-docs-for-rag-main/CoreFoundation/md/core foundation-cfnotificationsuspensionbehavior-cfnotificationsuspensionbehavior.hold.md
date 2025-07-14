

- Core Foundation
- CFNotificationSuspensionBehavior
-  CFNotificationSuspensionBehavior.hold 

Case

# CFNotificationSuspensionBehavior.hold

The server will hold all matching notifications until the queue has been filled (queue size determined by the server) at which point the server may flush queued notifications.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case hold
```

## See Also

### Constants

case drop

The server will not queue any notifications of the specified name and object while the receiving application is in the background.

case coalesce

The server will only queue the last notification of the specified name and object; earlier notifications are dropped.

case deliverImmediately

The server will deliver notifications of the specified name and object whether or not the application is in the background. When a notification with this suspension behavior is matched, it has the effect of first flushing any queued notifications.

