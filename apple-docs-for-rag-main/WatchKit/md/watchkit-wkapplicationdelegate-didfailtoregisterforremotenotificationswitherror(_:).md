

- WatchKit
- WKApplicationDelegate
-  didFailToRegisterForRemoteNotificationsWithError(\_:) 

Instance Method

# didFailToRegisterForRemoteNotificationsWithError(\_:)

Tells the delegate that Apple Push Notification service (APNs) can’t successfully complete the registration process.

watchOS 7.0+

``` source
@MainActor
optional func didFailToRegisterForRemoteNotificationsWithError(_ error: any Error)
```

## Parameters 

`error`  

An error object that contains information about why the registration failed. The app can choose to display this information to the user.

## Discussion

WatchKit calls this method if it was unable to register your app with APNs or if your app isn’t properly configured for remote notifications. For example, WatchKit might call this method if you didn’t enable your WatchKit extension’s Push Notification capability.\*\* \*\*For more information about how to set up and send remote notifications in your app, see Setting up a remote notification server and Registering your app with APNs.

In your implementation, you can check the error type, and try to register again later.

## See Also

### Managing remote notifications

func didRegisterForRemoteNotifications(withDeviceToken: Data)

Tells the delegate that the app successfully registered with Apple Push Notification service (APNs).

func didReceiveRemoteNotification([AnyHashable : Any], fetchCompletionHandler: (WKBackgroundFetchResult) -> Void)

Tells the delegate that a background notification has arrived.

enum WKBackgroundFetchResult

The result of an attempt to download the content associated with a remote notification.

