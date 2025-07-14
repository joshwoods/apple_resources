

- AppKit
- NSApplicationDelegate
-  application(\_:didRegisterForRemoteNotificationsWithDeviceToken:) 

Instance Method

# application(\_:didRegisterForRemoteNotificationsWithDeviceToken:)

Tells the delegate that the app registered for Apple Push Services.

macOS 10.7+

``` source
@MainActor
optional func application(
    _ application: NSApplication,
    didRegisterForRemoteNotificationsWithDeviceToken deviceToken: Data
)
```

## Parameters 

`application`  

The application that initiated the remote-notification registration process.

`deviceToken`  

A token that identifies the device to Apple Push Notification Service (APNS). The token is an opaque data type because that is the form that the provider needs to submit to the APNS servers when it sends a notification to a device. The APNS servers require a binary format for performance reasons.

The size of a device token is 32 bytes.

## Discussion

The delegate receives this message after the registerForRemoteNotifications(matching:)method of NSApplication is invoked and there is no error in the registration process. After receiving the device token, the application should connect with its provider and give the token to it. APNS only pushes notifications to the application’s computer that are accompanied with this token.

For more information about how to implement push notifications in your application, see Local and Remote Notification Programming Guide.

## See Also

### Handling Push Notifications

func application(NSApplication, didFailToRegisterForRemoteNotificationsWithError: any Error)

Tells the delegate that the app was unable to register for Apple Push Services.

func application(NSApplication, didReceiveRemoteNotification: [String : Any])

Tells the delegate when the app receives a remote notification.

