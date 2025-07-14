

- UIKit
- UIApplication
-  setMinimumBackgroundFetchInterval(\_:) Deprecated

Instance Method

# setMinimumBackgroundFetchInterval(\_:)

Specifies the minimum amount of time that must elapse between background fetch operations.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 11.0–13.0Deprecated

``` source
@MainActor
func setMinimumBackgroundFetchInterval(_ minimumBackgroundFetchInterval: TimeInterval)
```

Deprecated

For apps supporting iOS 13 and higher use BGAppRefreshTask.

## Parameters 

`minimumBackgroundFetchInterval`  

The minimum number of seconds that must elapse before another background fetch can be initiated. This value is advisory only and does not indicate the exact amount of time expected between fetch operations.

## Mentioned in 

Using background tasks to update your app

## Discussion

This property has no effect for apps that do not have the `UIBackgroundModes` key with the `fetch` value in its `Info.plist` file.

The default fetch interval for apps is backgroundFetchIntervalNever. Therefore, you must call this method and set a fetch interval before your app is given background execution time.

## See Also

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

func registerForRemoteNotifications(matching: UIRemoteNotificationType)

Register to receive remote notifications of the specified types via Apple Push Notification service.

Deprecated

