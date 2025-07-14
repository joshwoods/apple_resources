

- UIKit
- UIApplicationDelegate
-  application(\_:handleOpen:) Deprecated

Instance Method

# application(\_:handleOpen:)

Asks the delegate to open a resource identified by URL.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    handleOpen url: URL
) -> Bool
```

Deprecated

Use the application(_:open:options:) method instead.

## Parameters 

`application`  

Your singleton app object.

`url`  

An object representing a URL (Universal Resource Locator). See the appendix of App Programming Guide for iOS for Apple-registered schemes for URLs.

## Return Value

true if the delegate successfully handled the request; false if the attempt to handle the URL failed.

## Discussion

If the delegate also implements the application(_:open:sourceApplication:annotation:) method, that method is called instead of this one.

This method is not called if the delegate returns false from both the application(_:willFinishLaunchingWithOptions:) and application(_:didFinishLaunchingWithOptions:) methods. (If only one of the two methods is implemented, its return value determines whether this method is called.) If your app implements the applicationDidFinishLaunching(_:) method instead of application(_:didFinishLaunchingWithOptions:), this method is called to open the specified URL after the app has been initialized.

If a URL arrives while your app is suspended or running in the background, the system moves your app to the foreground prior to calling this method.

There is no equivalent notification for this delegation method.

## See Also

### Related Documentation

func application(UIApplication, didFinishLaunchingWithOptions: [UIApplication.LaunchOptionsKey : Any]?) -> Bool

Tells the delegate that the launch process is almost done and the app is almost ready to run.

func application(UIApplication, willFinishLaunchingWithOptions: [UIApplication.LaunchOptionsKey : Any]?) -> Bool

Tells the delegate that the launch process has begun.

func openURL(URL) -> Bool

Attempts to open the resource at the specified URL.

Deprecated

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

