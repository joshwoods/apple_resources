

- Core Foundation
- CFNotificationSuspensionBehavior
-  CFNotificationSuspensionBehavior.deliverImmediately 

Case

# CFNotificationSuspensionBehavior.deliverImmediately

The server will deliver notifications of the specified name and object whether or not the application is in the background. When a notification with this suspension behavior is matched, it has the effect of first flushing any queued notifications.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case deliverImmediately
```

## See Also

### Constants

case drop

The server will not queue any notifications of the specified name and object while the receiving application is in the background.

case coalesce

The server will only queue the last notification of the specified name and object; earlier notifications are dropped.

case hold

The server will hold all matching notifications until the queue has been filled (queue size determined by the server) at which point the server may flush queued notifications.

