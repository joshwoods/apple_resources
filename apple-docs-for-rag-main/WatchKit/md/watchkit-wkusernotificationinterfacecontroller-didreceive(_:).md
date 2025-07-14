

- WatchKit
- WKUserNotificationInterfaceController
-  didReceive(\_:) 

Instance Method

# didReceive(\_:)

Delivers a notification object to your interface controller for processing.

watchOS 5.0+

``` source
@MainActor
func didReceive(_ notification: UNNotification)
```

## See Also

### Processing the Notification

func didReceive(UNNotification, withCompletion: (WKUserNotificationInterfaceType) -> Void)

Delivers a notification object to your interface controller for processing.

Deprecated

