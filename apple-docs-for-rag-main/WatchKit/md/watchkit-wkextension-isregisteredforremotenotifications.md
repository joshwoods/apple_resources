

- WatchKit
- WKExtension
-  isRegisteredForRemoteNotifications 

Instance Property

# isRegisteredForRemoteNotifications

A Boolean value that indicates if the app has successfully registered for remote notifications.

watchOS 6.0+

``` source
@MainActor
var isRegisteredForRemoteNotifications: Bool { get }
```

## Discussion

This method indicates whether your app successfully registered for remote notifications using the registerForRemoteNotifications() method. It also takes into account the notification permissions set by the user. It does not give any indication about whether remote notifications are available.

## See Also

### Registering for remote notifications

func registerForRemoteNotifications()

Register to receive remote notifications from the Apple Push Notification service (APNs).

func unregisterForRemoteNotifications()

Unregister for all remote notifications received from Apple Push Notification service (APNs).

