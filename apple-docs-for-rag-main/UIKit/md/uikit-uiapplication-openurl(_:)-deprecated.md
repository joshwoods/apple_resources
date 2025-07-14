

- UIKit
- UIApplication
-  openURL(\_:) Deprecated

Instance Method

# openURL(\_:)

Attempts to open the resource at the specified URL.

iOS 2.0–10.0DeprecatediPadOS 2.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
func openURL(_ url: URL) -> Bool
```

Deprecated

Calling this method has no effect. Use the open(_:options:completionHandler:) method instead.

## Parameters 

`url`  

A URL (Universal Resource Locator). UIKit supports many common schemes, including the `http`, `https`, `tel`, `facetime`, and `mailto` schemes. You can also employ custom URL schemes associated with apps installed on the device.

## Return Value

true if the resource located by the URL was successfully opened; otherwise false.

## Discussion

The URL you pass to this method can identify a resource in the app that calls the method, or a resource to be handled by another app. If the resource is to be handled another app, invoking this method might cause the calling app to quit so the other can launch.

To check if there is an installed app that can handle a scheme, call the canOpenURL(_:) method before calling this one. Be sure to read the description of that method for an important note about registering the schemes you want to employ.

## See Also

### Related Documentation

func application(UIApplication, handleOpen: URL) -> Bool

Asks the delegate to open a resource identified by URL.

Deprecated

func canOpenURL(URL) -> Bool

Returns a Boolean value that indicates whether an app is available to handle a URL scheme.

### Deprecated methods

func requestSceneSessionActivation(UISceneSession?, userActivity: NSUserActivity?, options: UIScene.ActivationRequestOptions?, errorHandler: ((any Error) -> Void)?)

Asks the system to activate an existing scene, or create a new scene and associate it with your app.

Deprecated

func beginIgnoringInteractionEvents()

Tells the receiver to suspend the handling of touch-related events.

Deprecated

func endIgnoringInteractionEvents()

Tells the receiver to resume the handling of touch-related events.

Deprecated

func setMinimumBackgroundFetchInterval(TimeInterval)

Specifies the minimum amount of time that must elapse between background fetch operations.

Deprecated

func scheduleLocalNotification(UILocalNotification)

Schedules a local notification for delivery at its encapsulated date and time.

Deprecated

func presentLocalNotificationNow(UILocalNotification)

Presents a local notification immediately.

Deprecated

func cancelLocalNotification(UILocalNotification)

Cancels the delivery of the specified scheduled local notification.

Deprecated

func cancelAllLocalNotifications()

Cancels the delivery of all scheduled local notifications.

Deprecated

func setKeepAliveTimeout(TimeInterval, handler: (() -> Void)?) -> Bool

Configures a periodic handler for VoIP apps in older versions of iOS.

Deprecated

let UIMinimumKeepAliveTimeout: TimeInterval

The minimum amount of time (measured in seconds) an app may run a critical background task in the background.

Deprecated

func clearKeepAliveTimeout()

Removes a previously installed periodic handler block.

Deprecated

func setStatusBarHidden(Bool, with: UIStatusBarAnimation)

Hides or shows the status bar, optionally animating the transition.

Deprecated

func setStatusBarStyle(UIStatusBarStyle, animated: Bool)

Sets the style of the status bar, optionally animating the transition to the new style.

Deprecated

func setStatusBarOrientation(UIInterfaceOrientation, animated: Bool)

Sets the app’s status bar to the specified orientation, optionally animating the transition.

Deprecated

func registerUserNotificationSettings(UIUserNotificationSettings)

Registers your preferred options for notifying the user.

Deprecated

