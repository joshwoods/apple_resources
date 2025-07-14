

- UIKit
- UIApplicationDelegate
-  application(\_:didChangeStatusBarOrientation:) Deprecated

Instance Method

# application(\_:didChangeStatusBarOrientation:)

Tells the delegate when the interface orientation of the status bar has changed.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    didChangeStatusBarOrientation oldStatusBarOrientation: UIInterfaceOrientation
)
```

## Parameters 

`application`  

Your singleton app object.

`oldStatusBarOrientation`  

A constant that indicates the previous orientation of the app’s user interface; see Responding to app life-cycle events for details.

## Discussion

The delegate can get the current device orientation from the shared UIDevice object.

After calling this method, the app also posts a didChangeStatusBarOrientationNotification notification to give interested objects a chance to respond to the change.

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

