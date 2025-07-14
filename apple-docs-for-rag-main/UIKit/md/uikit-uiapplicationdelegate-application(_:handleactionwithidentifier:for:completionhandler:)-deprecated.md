

- UIKit
- UIApplicationDelegate
-  application(\_:handleActionWithIdentifier:for:completionHandler:) Deprecated

Instance Method

# application(\_:handleActionWithIdentifier:for:completionHandler:)

Called when your app has been activated because user selected a custom action from the alert panel of a local notification.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

**iOS, iPadOS, Mac Catalyst**

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    handleActionWithIdentifier identifier: String?,
    for notification: UILocalNotification,
    completionHandler: @escaping () -> Void
)
```

**Mac Catalyst**

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    handleActionWithIdentifier identifier: String?,
    for notification: UILocalNotification
) async
```

Deprecated

Use userNotificationCenter(_:didReceive:withCompletionHandler:) instead.

## Parameters 

`application`  

The app object that received the local notification.

`identifier`  

The identifier associated with the custom action. This string corresponds to the identifier from the UILocalNotificationAction object that was used to configure the action in the local notification.

`notification`  

The local notification object that was triggered.

`completionHandler`  

A block to call when you are finished performing the action.

## Discussion

The app calls this method when the user taps an action button in an alert displayed in response to a local notification. Local notifications that include a registered category name in their category property display buttons for the actions in that category. If the user taps one of those buttons, the system wakes up the app (launching it if needed) and calls this method in the background. Your implementation of this method should perform the action associated with the specified `identifier` and execute the block in the `completionHandler` parameter as soon as you are done. Failure to execute the completion handler block at the end of your implementation will cause your app to be terminated.

To configure the actions for a given category, create a UIUserNotificationActionSettings object and register it with the app when you call the registerUserNotificationSettings(_:) method.

## See Also

### Deprecated

func application(UIApplication, didRegister: UIUserNotificationSettings)

Called to tell the delegate the types of local and remote notifications that can be used to get the user’s attention.

Deprecated

func application(UIApplication, didReceive: UILocalNotification)

Sent to the delegate when a running app receives a local notification.

Deprecated

func application(UIApplication, didReceiveRemoteNotification: [AnyHashable : Any])

Called when your app has received a remote notification.

Deprecated

func application(UIApplication, handleActionWithIdentifier: String?, for: UILocalNotification, withResponseInfo: [AnyHashable : Any], completionHandler: () -> Void)

Called when your app has been activated by the user selecting an action from a local notification.

Deprecated

func application(UIApplication, handleActionWithIdentifier: String?, forRemoteNotification: [AnyHashable : Any], completionHandler: () -> Void)

Tells the app delegate to perform the custom action specified by a remote notification.

Deprecated

func application(UIApplication, handleActionWithIdentifier: String?, forRemoteNotification: [AnyHashable : Any], withResponseInfo: [AnyHashable : Any], completionHandler: () -> Void)

Called when your app has been activated by the user selecting an action from a remote notification.

Deprecated

func application(UIApplication, handleOpen: URL) -> Bool

Asks the delegate to open a resource identified by URL.

Deprecated

func application(UIApplication, open: URL, sourceApplication: String?, annotation: Any) -> Bool

Asks the delegate to open a resource identified by a URL.

Deprecated

func application(UIApplication, willChangeStatusBarOrientation: UIInterfaceOrientation, duration: TimeInterval)

Tells the delegate when the interface orientation of the status bar is about to change.

Deprecated

func application(UIApplication, didChangeStatusBarOrientation: UIInterfaceOrientation)

Tells the delegate when the interface orientation of the status bar has changed.

Deprecated

func application(UIApplication, willChangeStatusBarFrame: CGRect)

Tells the delegate when the frame of the status bar is about to change.

Deprecated

func application(UIApplication, didChangeStatusBarFrame: CGRect)

Tells the delegate when the frame of the status bar has changed.

Deprecated

func application(UIApplication, handle: INIntent, completionHandler: (INIntentResponse) -> Void)

Asks the delegate to handle the specified SiriKit intent directly.

Deprecated

func application(UIApplication, performFetchWithCompletionHandler: (UIBackgroundFetchResult) -> Void)

Tells the app that it can begin a fetch operation if it has data to download.

Deprecated

func application(UIApplication, shouldSaveApplicationState: NSCoder) -> Bool

Asks the delegate whether to preserve the app’s state.

Deprecated

