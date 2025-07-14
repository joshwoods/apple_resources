

- UIKit
- UIApplication
-  registerForRemoteNotifications() 

Instance Method

# registerForRemoteNotifications()

Registers to receive remote notifications through Apple Push Notification service.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func registerForRemoteNotifications()
```

## Discussion

Call this method to initiate the registration process with Apple Push Notification service. If registration succeeds, the app calls your app delegate object’s application(_:didRegisterForRemoteNotificationsWithDeviceToken:) method and passes it a device token. You should pass this token along to the server you use to generate remote notifications for the device. If registration fails, the app calls its app delegate’s application(_:didFailToRegisterForRemoteNotificationsWithError:) method instead.

If you want your app’s remote notifications to display alerts, play sounds, or perform other user-facing actions, you must request authorization to do so using the requestAuthorization(options:completionHandler:) method of UNUserNotificationCenter. If you do not request and receive authorization for your app’s interactions, the system delivers all remote notifications to your app silently.

## See Also

### Registering for remote notifications

func unregisterForRemoteNotifications()

Unregisters for all remote notifications received through Apple Push Notification service.

var isRegisteredForRemoteNotifications: Bool

A Boolean value that indicates whether the app is currently registered for remote notifications.

