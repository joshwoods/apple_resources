

- UIKit
- UIApplication
-  unregisterForRemoteNotifications() 

Instance Method

# unregisterForRemoteNotifications()

Unregisters for all remote notifications received through Apple Push Notification service.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func unregisterForRemoteNotifications()
```

## Discussion

You should call this method in rare circumstances only, such as when a new version of the app removes support for all types of remote notifications. Users can temporarily prevent apps from receiving remote notifications through the Notifications section of the Settings app. Apps unregistered through this method can always re-register.

## See Also

### Registering for remote notifications

func registerForRemoteNotifications()

Registers to receive remote notifications through Apple Push Notification service.

var isRegisteredForRemoteNotifications: Bool

A Boolean value that indicates whether the app is currently registered for remote notifications.

