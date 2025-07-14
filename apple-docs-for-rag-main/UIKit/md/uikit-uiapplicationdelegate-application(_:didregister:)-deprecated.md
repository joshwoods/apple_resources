

- UIKit
- UIApplicationDelegate
-  application(\_:didRegister:) Deprecated

Instance Method

# application(\_:didRegister:)

Called to tell the delegate the types of local and remote notifications that can be used to get the user’s attention.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    didRegister notificationSettings: UIUserNotificationSettings
)
```

Deprecated

Use requestAuthorization(options:completionHandler:) instead.

## Parameters 

`application`  

The app object that registered the user notification settings.

`notificationSettings`  

The user’s specified notification settings for your app. The settings in this object may be different than the ones you originally requested.

## Discussion

Apps that use local or remote notifications to alert the user to new information must register the types of notifications they want to use by calling the registerUserNotificationSettings(_:) method of the app object. The system compares your app’s request with the user’s preferences to determine the types of local and remote notifications allowed, and returns the results to your app by calling this method. Check the contents of the `notificationSettings` parameter whenever this method is called.

Because the user can change notification settings in the Settings app at any time, call the currentUserNotificationSettings method before your app performs work to prepare a notification for presentation.

The first time you register your app’s preferred notification types, the system asks the user whether your app should be allowed to deliver notifications and stores the user’s response. The system does not prompt the user on subsequent calls to the registerUserNotificationSettings(_:) method, but the user can always change notification preferences using Settings.

A user’s notification settings control only whether the system *displays* local or remote notifications onscreen. Regardless of the notification settings, local and remote notifications are delivered to your app at the appropriate times.

## See Also

### Deprecated

func application(UIApplication, didReceive: UILocalNotification)

Sent to the delegate when a running app receives a local notification.

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

