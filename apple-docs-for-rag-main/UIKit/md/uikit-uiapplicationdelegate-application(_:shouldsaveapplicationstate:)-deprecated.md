

- UIKit
- UIApplicationDelegate
-  application(\_:shouldSaveApplicationState:) Deprecated

Instance Method

# application(\_:shouldSaveApplicationState:)

Asks the delegate whether to preserve the app’s state.

iOS 6.0–13.2DeprecatediPadOS 6.0–13.2DeprecatedMac Catalyst 13.1–13.2DeprecatedtvOSDeprecated

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    shouldSaveApplicationState coder: NSCoder
) -> Bool
```

Deprecated

Use application(_:shouldSaveSecureApplicationState:) instead.

## Parameters 

`application`  

Your singleton app object.

`coder`  

The keyed archiver into which you can put high-level state information.

## Return Value

true if the app’s state should be preserved; otherwise, false.

## Discussion

Apps must implement this method and the application(_:shouldRestoreApplicationState:) method for state preservation to occur. In addition, your implementation of this method must return true each time UIKit tries to preserve the state of your app. You can return false to disable state preservation temporarily. For example, during testing, you could disable state preservation to test specific code paths.

You can add version information or any other contextual data to the provided coder object as needed. During restoration, you can use that information to help decide whether or not to proceed with restoring your app to its previous state.

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

