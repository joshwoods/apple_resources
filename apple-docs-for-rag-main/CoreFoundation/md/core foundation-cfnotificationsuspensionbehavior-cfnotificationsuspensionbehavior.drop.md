

- Core Foundation
- CFNotificationSuspensionBehavior
-  CFNotificationSuspensionBehavior.drop 

Case

# CFNotificationSuspensionBehavior.drop

The server will not queue any notifications of the specified name and object while the receiving application is in the background.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case drop
```

## See Also

### Constants

case coalesce

The server will only queue the last notification of the specified name and object; earlier notifications are dropped.

case hold

The server will hold all matching notifications until the queue has been filled (queue size determined by the server) at which point the server may flush queued notifications.

case deliverImmediately

The server will deliver notifications of the specified name and object whether or not the application is in the background. When a notification with this suspension behavior is matched, it has the effect of first flushing any queued notifications.

