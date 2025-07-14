

- WatchKit
- WKApplication
-  unregisterForRemoteNotifications() 

Instance Method

# unregisterForRemoteNotifications()

Unregister for all remote notifications received from Apple Push Notification service (APNs).

watchOS 7.0+

``` source
@MainActor
func unregisterForRemoteNotifications()
```

## Discussion

Use this method to unregister from all remote notifications; for example, unregister to stop receiving notifications when the user logs out of their account.

## See Also

### Related Documentation

@MainActor func registerForRemoteNotifications()

Registers to receive remote notifications through Apple Push Notification service.

### Registering for remote notifications

func registerForRemoteNotifications()

Register to receive remote notifications from the Apple Push Notification service (APNs).

var isRegisteredForRemoteNotifications: Bool

A Boolean value that indicates if the app has successfully registered for remote notifications.

