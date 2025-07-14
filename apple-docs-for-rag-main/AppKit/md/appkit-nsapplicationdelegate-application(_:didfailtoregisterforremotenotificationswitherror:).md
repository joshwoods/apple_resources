

- AppKit
- NSApplicationDelegate
-  application(\_:didFailToRegisterForRemoteNotificationsWithError:) 

Instance Method

# application(\_:didFailToRegisterForRemoteNotificationsWithError:)

Tells the delegate that the app was unable to register for Apple Push Services.

macOS 10.7+

``` source
@MainActor
optional func application(
    _ application: NSApplication,
    didFailToRegisterForRemoteNotificationsWithError error: any Error
)
```

## Parameters 

`application`  

The application that initiated the remote-notification registration process.

`error`  

An NSError object that encapsulates information why registration did not succeed. The application can display this information to the user.

## Discussion

The delegate receives this message after the registerForRemoteNotifications(matching:) method of NSApplication is invoked and there is an error in the registration process.

For more information about how to implement push notifications in your application, see Local and Remote Notification Programming Guide.

## See Also

### Handling Push Notifications

func application(NSApplication, didRegisterForRemoteNotificationsWithDeviceToken: Data)

Tells the delegate that the app registered for Apple Push Services.

func application(NSApplication, didReceiveRemoteNotification: [String : Any])

Tells the delegate when the app receives a remote notification.

