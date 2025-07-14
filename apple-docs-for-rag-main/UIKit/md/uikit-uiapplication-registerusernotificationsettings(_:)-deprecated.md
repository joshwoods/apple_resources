

- UIKit
- UIApplication
-  registerUserNotificationSettings(\_:) Deprecated

Instance Method

# registerUserNotificationSettings(\_:)

Registers your preferred options for notifying the user.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func registerUserNotificationSettings(_ notificationSettings: UIUserNotificationSettings)
```

Deprecated

Use requestAuthorization(options:completionHandler:) and setNotificationCategories(_:) instead.

## Parameters 

`notificationSettings`  

The types of notifications that your app wants to use. You also use this object to specify custom actions that can be initiated by the user from an alert displayed in response to a local or remote notification.

## Discussion

If your app displays alerts, play sounds, or badges its icon, you must call this method during your launch cycle to request permission to alert the user in these ways. (You must also make this request if you want to set the applicationIconBadgeNumber property directly.) Typically, you make this request if your app uses local or remote notifications to alert the user to new information involving your app. The first time your app launches and calls this method, the system asks the user whether your app should be allowed to deliver notifications and stores the response. Thereafter, the system uses the stored response to determine the actual types of notifications you may use.

After calling this method, the app calls the application(_:didRegister:) method of its app delegate to report the results. You can use that method to determine if your request was granted or denied by the user.

It is recommended that you call this method before you schedule any local notifications or register with the push notification service. Apps that support custom actions must include all of their supported actions in the `notificationSettings` object.

## See Also

### Related Documentation

var currentUserNotificationSettings: UIUserNotificationSettings?

Returns the user notification settings for the app.

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

func setStatusBarStyle(UIStatusBarStyle, animated: Bool)

Sets the style of the status bar, optionally animating the transition to the new style.

Deprecated

func setStatusBarOrientation(UIInterfaceOrientation, animated: Bool)

Sets the app’s status bar to the specified orientation, optionally animating the transition.

Deprecated

func registerForRemoteNotifications(matching: UIRemoteNotificationType)

Register to receive remote notifications of the specified types via Apple Push Notification service.

Deprecated

