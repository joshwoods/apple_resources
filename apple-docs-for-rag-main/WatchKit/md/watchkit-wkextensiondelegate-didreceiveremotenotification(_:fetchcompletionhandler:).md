

- WatchKit
- WKExtensionDelegate
-  didReceiveRemoteNotification(\_:fetchCompletionHandler:) 

Instance Method

# didReceiveRemoteNotification(\_:fetchCompletionHandler:)

Tells the delegate that a background notification has arrived.

watchOS 6.0+

``` source
@MainActor
optional func didReceiveRemoteNotification(
    _ userInfo: [AnyHashable : Any],
    fetchCompletionHandler completionHandler: @escaping (WKBackgroundFetchResult) -> Void
)
```

``` source
@MainActor
optional func didReceiveRemoteNotification(_ userInfo: [AnyHashable : Any]) async -> WKBackgroundFetchResult
```

## Parameters 

`userInfo`  

A dictionary that contains data from the notification payload. The notification originates as a JSON-defined dictionary that WatchKit converts to a dictionary type; the dictionary may contain only property-list objects plus NSNull. For more information about the contents of the notification payload, see Generating a remote notification.

`completionHandler`  

The block to execute after the download operation completes. When calling this block, pass the fetch result that best describes your download operation. For a list of possible values, see the WKBackgroundFetchResult type.

## Discussion

Implement this method to process incoming background notifications. The system launches your app or wakes it from the suspended state when the notification arrives, and your app receives a brief amount of time to run in the background.

Use the background execution time to process the notification and download its associated content. As soon as you finish processing the notification, you must call its fetch completion handler. Your app has up to 30 seconds of wall-clock time to process the notification and call the handler or the system terminates your app. Always call the handler as quickly as possible, because the system tracks the elapsed time, power usage, and data costs for your app’s background notifications.

Background notifications are low priority, and the system limits these notifications based on the power considerations of the target device. APNs doesn’t guarantee that a device will receive push notifications, and apps that use significant amounts of power or time when processing background notifications may not receive background time to process future notifications.

For more information, see Pushing background updates to your App.

## See Also

### Managing remote notifications

func didRegisterForRemoteNotifications(withDeviceToken: Data)

Tells the delegate that the app successfully registered with Apple Push Notification service (APNs).

func didFailToRegisterForRemoteNotificationsWithError(any Error)

Tells the delegate that Apple Push Notification service (APNs) cannot successfully complete the registration process.

enum WKBackgroundFetchResult

The result of an attempt to download the content associated with a remote notification.

