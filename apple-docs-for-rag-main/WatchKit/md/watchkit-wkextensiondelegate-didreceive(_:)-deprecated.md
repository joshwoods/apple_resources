

- WatchKit
- WKExtensionDelegate
-  didReceive(\_:) Deprecated

Instance Method

# didReceive(\_:)

Tells the delegate that a local notification was triggered.

watchOS 2.0–3.0Deprecated

``` source
@MainActor
optional func didReceive(_ notification: UILocalNotification)
```

Deprecated

Instead of using this method, create a delegate object that adopts the UNUserNotificationCenterDelegate protocol and implement the `userNotificationCenter:willPresentNotification:withCompletionHandler:` and `userNotificationCenter:didReceiveNotificationResponse:withCompletionHandler:` methods. Assign this object to the `delegate` property of the singleton UNUserNotificationCenter object.

## Parameters 

`notification`  

The local notification object corresponding to the event that was triggered.

## Discussion

If a local notification arrives while your app is active, WatchKit calls this method to deliver the notification payload. Use this method to respond to the notification. For example, you might use this method to update your app’s interface or display a message to the user.

WatchKit may call this method multiple times. If a new local notification with the same category arrives while your app is active, WatchKit calls the method again with the new payload.

## See Also

### Deprecated Methods

func didReceiveRemoteNotification([AnyHashable : Any])

Tells the delegate that a remote notification arrived.

Deprecated

func handleAction(withIdentifier: String?, forRemoteNotification: [AnyHashable : Any])

Delivers a remote notification payload and a user-selected action to the app.

Deprecated

func handleAction(withIdentifier: String?, forRemoteNotification: [AnyHashable : Any], withResponseInfo: [AnyHashable : Any])

Delivers a remote notification payload and user response information to the app.

Deprecated

func handleAction(withIdentifier: String?, for: UILocalNotification)

Delivers a local notification payload and a user-selected action to the app.

Deprecated

func handleAction(withIdentifier: String?, for: UILocalNotification, withResponseInfo: [AnyHashable : Any])

Delivers a local notification payload and user response information to the app.

Deprecated

