

- WatchKit
- WKExtensionDelegate
-  handleAction(withIdentifier:for:withResponseInfo:) Deprecated

Instance Method

# handleAction(withIdentifier:for:withResponseInfo:)

Delivers a local notification payload and user response information to the app.

watchOS 2.0–3.0Deprecated

``` source
@MainActor
optional func handleAction(
    withIdentifier identifier: String?,
    for localNotification: UILocalNotification,
    withResponseInfo responseInfo: [AnyHashable : Any]
)
```

Deprecated

Instead of using this method, create a delegate object that adopts the UNUserNotificationCenterDelegate protocol and implement the `userNotificationCenter:willPresentNotification:withCompletionHandler:` and `userNotificationCenter:didReceiveNotificationResponse:withCompletionHandler:` methods. Assign this object to the `delegate` property of the singleton UNUserNotificationCenter object.

## Parameters 

`identifier`  

The action selected by the user. This string is the identifier assigned to the action at registration time. This parameter is set to the empty string when the user launches the app without tapping one of the action buttons.

`localNotification`  

The local notification object that triggered the notification.

`responseInfo`  

The response information dictionary. This dictionary contains the UIUserNotificationActionResponseTypedTextKey key with the text response selected by the user.

## Discussion

Use this method to handle actions selected by users from your notification interfaces. If your containing iOS app supports interactive notifications, the `identifier` parameter may contain the action identifier for the button that was tapped. Use that value to perform the requested action. If the `identifier` parameter contains an empty string, that means the user launched your Watch app from the notification interface without choosing a specific action.

The system calls this method on your WatchKit extension’s main thread. The `super` implementation of this method does nothing.

For information about how to support interactive notifications in your iOS app, see Local and Remote Notification Programming Guide. For information about how to display a custom interface for notifications, see App Programming Guide for watchOS.

## See Also

### Deprecated Methods

func didReceiveRemoteNotification([AnyHashable : Any])

Tells the delegate that a remote notification arrived.

Deprecated

func didReceive(UILocalNotification)

Tells the delegate that a local notification was triggered.

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

