

- UIKit
- UIApplicationDelegate
-  application(\_:didReceiveRemoteNotification:) Deprecated

Instance Method

# application(\_:didReceiveRemoteNotification:)

Called when your app has received a remote notification.

iOS 3.0–10.0DeprecatediPadOS 3.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    didReceiveRemoteNotification userInfo: [AnyHashable : Any]
)
```

Deprecated

Use application(_:didReceiveRemoteNotification:fetchCompletionHandler:) instead.

## Parameters 

`application`  

The app object that received the remote notification.

`userInfo`  

A dictionary that contains information related to the remote notification, potentially including a badge number for the app icon, an alert sound, an alert message to display to the user, a notification identifier, and custom data. The provider originates it as a JSON-defined dictionary that iOS converts to an NSDictionary object; the dictionary might contain only property-list objects plus NSNull.

## Discussion

Implement the application(_:didReceiveRemoteNotification:fetchCompletionHandler:) method instead of this one whenever possible. If your delegate implements both methods, the app object calls the application(_:didReceiveRemoteNotification:fetchCompletionHandler:) method.

If the app is running, the app calls this method to process incoming remote notifications. The `userInfo` dictionary contains the `aps` key whose value is another dictionary with the remaining notification data. Although you should not need the information in the `aps` dictionary, you can retrieve its contents using the following keys:

- `alert`—The value is either a string for the alert message or a dictionary with two keys: `body` and `show-view`. The value of the `body` key is a string containing the alert message and the value of the `show-view` key is a Boolean. If the value of the `show-view` key is `false`, the alert’s View button is not shown. The default is to show the View button which, if the user taps it, launches the app.

- `badge`—A number indicating the quantity of data items to download from the provider. This number is to be displayed on the app icon. The absence of a `badge` property indicates that any number currently badging the icon should be removed.

- `sound`—The name of a sound file in the app bundle to play as an alert sound. If “default” is specified, the default sound should be played.

The `userInfo` dictionary may also have custom data defined by the provider according to the JSON schema. The properties for custom data should be specified at the same level as the `aps` dictionary. However, custom-defined properties should not be used for mass data transport because there is a strict size limit per notification (256 bytes) and delivery is not guaranteed.

If the app is not running when a remote notification arrives, the method launches the app and provides the appropriate information in the launch options dictionary. The app does not call this method to handle that remote notification. Instead, your implementation of the application(_:willFinishLaunchingWithOptions:) or application(_:didFinishLaunchingWithOptions:) method needs to get the remote notification payload data and respond appropriately.

For more information about how to implement remote notifications in your app, see Local and Remote Notification Programming Guide.

## See Also

### Related Documentation

func application(UIApplication, didRegisterForRemoteNotificationsWithDeviceToken: Data)

Tells the delegate that the app successfully registered with Apple Push Notification service (APNs).

func application(UIApplication, didFailToRegisterForRemoteNotificationsWithError: any Error)

Tells the delegate when Apple Push Notification service cannot successfully complete the registration process.

### Deprecated

func application(UIApplication, didRegister: UIUserNotificationSettings)

Called to tell the delegate the types of local and remote notifications that can be used to get the user’s attention.

Deprecated

func application(UIApplication, didReceive: UILocalNotification)

Sent to the delegate when a running app receives a local notification.

Deprecated

func application(UIApplication, handleActionWithIdentifier: String?, for: UILocalNotification, completionHandler: () -> Void)

Called when your app has been activated because user selected a custom action from the alert panel of a local notification.

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

