

- WatchKit
- WKExtensionDelegate
-  didRegisterForRemoteNotifications(withDeviceToken:) 

Instance Method

# didRegisterForRemoteNotifications(withDeviceToken:)

Tells the delegate that the app successfully registered with Apple Push Notification service (APNs).

watchOS 6.0+

``` source
@MainActor
optional func didRegisterForRemoteNotifications(withDeviceToken deviceToken: Data)
```

## Parameters 

`deviceToken`  

A globally unique token that identifies this device to APNs. Send this token to the server that you use to generate remote notifications. Your server must pass this token unmodified back to APNs when sending notifications to this device.

The length of APNs device tokens can vary. Do not hardcode the token’s size in your app.

## Discussion

WatchKit calls this method after it successfully registers your app with APNs. In your implementation, send the contents of the `deviceToken` parameter to the server you use to generate remote notifications. Never cache the device token locally on the user’s device. Device tokens can change periodically, so caching the value risks sending an invalid token to your server.

Typically, the system calls this method only after you call your WKExtension object’s registerForRemoteNotifications() method, but WatchKit may call it under other rare circumstances. For example, WatchKit calls the method when the user launches an app after setting up the watch using a different device’s backup. In this case, the app doesn’t know the new device’s token until the user launches it.

## See Also

### Related Documentation

@MainActor optional func application(_ application: UIApplication, didFailToRegisterForRemoteNotificationsWithError error: any Error)

Tells the delegate when Apple Push Notification service cannot successfully complete the registration process.

@MainActor optional func application(_ application: UIApplication, didReceiveRemoteNotification userInfo: [AnyHashable : Any])

Called when your app has received a remote notification.

Deprecated

@MainActor func registerForRemoteNotifications()

Registers to receive remote notifications through Apple Push Notification service.

### Managing remote notifications

func didFailToRegisterForRemoteNotificationsWithError(any Error)

Tells the delegate that Apple Push Notification service (APNs) cannot successfully complete the registration process.

func didReceiveRemoteNotification([AnyHashable : Any], fetchCompletionHandler: (WKBackgroundFetchResult) -> Void)

Tells the delegate that a background notification has arrived.

enum WKBackgroundFetchResult

The result of an attempt to download the content associated with a remote notification.

