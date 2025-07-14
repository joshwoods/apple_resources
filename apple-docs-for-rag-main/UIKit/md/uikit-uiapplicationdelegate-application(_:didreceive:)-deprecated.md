

- UIKit
- UIApplicationDelegate
-  application(\_:didReceive:) Deprecated

Instance Method

# application(\_:didReceive:)

Sent to the delegate when a running app receives a local notification.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    didReceive notification: UILocalNotification
)
```

Deprecated

Use userNotificationCenter(_:willPresent:withCompletionHandler:) instead.

## Parameters 

`application`  

The app object that received the local notification.

`notification`  

A local notification that encapsulates details about the notification, potentially including custom data.

## Discussion

Local notifications are similar to remote notifications, but differ in that they are scheduled, displayed, and received entirely on the same device. An app can create and schedule a local notification, and the operating system then delivers it at the scheduled date and time. If the app is not active in the foreground when the notification fires, the system uses the information in the UILocalNotification object to determine whether it should display an alert, badge the app icon, or play a sound. If the app is running in the foreground, the system calls this method directly without alerting the user in any way.

You might implement this method in your delegate if you want to be notified that a local notification occurred. For example, a calendar app might use local notifications to alert the user to upcoming events.

If the user chooses to open the app when a local notification occurs, the launch options dictionary passed to the application(_:willFinishLaunchingWithOptions:) and application(_:didFinishLaunchingWithOptions:) methods contains the localNotification key. This method is called at some point after your delegate’s application(_:didFinishLaunchingWithOptions:) method.

## See Also

### Deprecated

func application(UIApplication, didRegister: UIUserNotificationSettings)

Called to tell the delegate the types of local and remote notifications that can be used to get the user’s attention.

Deprecated

func application(UIApplication, didReceiveRemoteNotification: [AnyHashable : Any])

Called when your app has received a remote notification.

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

