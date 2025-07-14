

- UIKit
- UIApplication
-  scheduleLocalNotification(\_:) Deprecated

Instance Method

# scheduleLocalNotification(\_:)

Schedules a local notification for delivery at its encapsulated date and time.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func scheduleLocalNotification(_ notification: UILocalNotification)
```

Deprecated

Use the UNUserNotificationCenter class to schedule local notifications instead.

## Parameters 

`notification`  

The local notification object that you want to schedule. This object contains information about when to deliver the notification and what to do when that date occurs. The system keeps a copy of this object so you may release the object once it is scheduled.

## Discussion

Prior to scheduling any local notifications, you must call the registerUserNotificationSettings(_:) method to let the system know what types of alerts, if any, you plan to display to the user.

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

func setMinimumBackgroundFetchInterval(TimeInterval)

Specifies the minimum amount of time that must elapse between background fetch operations.

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

