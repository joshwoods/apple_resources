

- UIKit
- UIApplication
-  isRegisteredForRemoteNotifications 

Instance Property

# isRegisteredForRemoteNotifications

A Boolean value that indicates whether the app is currently registered for remote notifications.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isRegisteredForRemoteNotifications: Bool { get }
```

## Discussion

This method reflects whether the remote registration process completed successfully—a process that begins when you call the registerForRemoteNotifications() method. This method does not reflect whether remote notifications are actually available due to connectivity issues. The value returned by this method takes into account the user’s preferences for receiving remote notifications.

## See Also

### Registering for remote notifications

func registerForRemoteNotifications()

Registers to receive remote notifications through Apple Push Notification service.

func unregisterForRemoteNotifications()

Unregisters for all remote notifications received through Apple Push Notification service.

