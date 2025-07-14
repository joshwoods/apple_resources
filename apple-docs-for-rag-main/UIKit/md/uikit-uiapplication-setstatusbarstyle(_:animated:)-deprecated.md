

- UIKit
- UIApplication
-  setStatusBarStyle(\_:animated:) Deprecated

Instance Method

# setStatusBarStyle(\_:animated:)

Sets the style of the status bar, optionally animating the transition to the new style.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func setStatusBarStyle(
    _ statusBarStyle: UIStatusBarStyle,
    animated: Bool
)
```

## Parameters 

`statusBarStyle`  

A constant that specifies a style for the status bar. See the descriptions of the constants in UIStatusBarStyle for details.

`animated`  

true if the transition to the new style should be animated; otherwise false .

## Discussion

The animation slides the status bar out toward the top of the interface.

In iOS 7 and later, status bar behavior is determined by view controllers, and so calling this method has no effect by default. When view controller-based status bar appearance is disabled, this method behaves normally. To opt out of the view controller-based status bar appearance behavior, you must add the `UIViewControllerBasedStatusBarAppearance` key with a value of false to your app’s `Info.plist` file, but doing so is not recommended.

## See Also

### Related Documentation

var statusBarStyle: UIStatusBarStyle

The current style of the status bar.

Deprecated

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

func setStatusBarOrientation(UIInterfaceOrientation, animated: Bool)

Sets the app’s status bar to the specified orientation, optionally animating the transition.

Deprecated

func registerUserNotificationSettings(UIUserNotificationSettings)

Registers your preferred options for notifying the user.

Deprecated

func registerForRemoteNotifications(matching: UIRemoteNotificationType)

Register to receive remote notifications of the specified types via Apple Push Notification service.

Deprecated

