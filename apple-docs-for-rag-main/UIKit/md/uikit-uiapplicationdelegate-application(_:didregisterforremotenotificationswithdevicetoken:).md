

- UIKit
- UIApplicationDelegate
-  application(\_:didRegisterForRemoteNotificationsWithDeviceToken:) 

Instance Method

# application(\_:didRegisterForRemoteNotificationsWithDeviceToken:)

Tells the delegate that the app successfully registered with Apple Push Notification service (APNs).

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    didRegisterForRemoteNotificationsWithDeviceToken deviceToken: Data
)
```

## Parameters 

`application`  

The app object that initiated the remote-notification registration process.

`deviceToken`  

A globally unique token that identifies this device to APNs. Send this token to the server that you use to generate remote notifications. Your server must pass this token unmodified back to APNs when sending those remote notifications.

APNs device tokens are of variable length. Do not hard-code their size.

## Discussion

UIKit calls this method after it successfully registers your app with APNs. In your implementation of this method, send the contents of the `deviceToken` parameter to the server that you use to generate remote notifications. Never cache the device token locally on the user’s device. Device tokens can change periodically, so caching the value risks sending an invalid token to your server. If the device token hasn’t changed, registering with APNs and returning the token happens quickly.

Typically, this method is called only after you call the registerForRemoteNotifications() method of UIApplication, but UIKit might call it in other rare circumstances. For example, UIKit calls the method when the user launches an app after having restored a device from data that is not the device’s backup data. In this exceptional case, the app won’t know the new device’s token until the user launches it.

## See Also

### Related Documentation

func application(UIApplication, didReceiveRemoteNotification: [AnyHashable : Any])

Called when your app has received a remote notification.

Deprecated

func registerForRemoteNotifications()

Registers to receive remote notifications through Apple Push Notification service.

### Handling remote notification registration

func application(UIApplication, didFailToRegisterForRemoteNotificationsWithError: any Error)

Tells the delegate when Apple Push Notification service cannot successfully complete the registration process.

func application(UIApplication, didReceiveRemoteNotification: [AnyHashable : Any], fetchCompletionHandler: (UIBackgroundFetchResult) -> Void)

Tells the app that a remote notification arrived that indicates there is data to be fetched.

