

- UIKit
- UIApplication
-  registerForRemoteNotifications(matching:) Deprecated

Instance Method

# registerForRemoteNotifications(matching:)

Register to receive remote notifications of the specified types via Apple Push Notification service.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func registerForRemoteNotifications(matching types: UIRemoteNotificationType)
```

Deprecated

Use the registerForRemoteNotifications() method instead.

## Parameters 

`types`  

A bit mask specifying the types of notifications the app accepts. For a list of values, see UIRemoteNotificationType.

## Discussion

When you send this message, the device initiates the registration process with Apple Push Notification service. If it succeeds, the app delegate receives a device token in the application(_:didRegisterForRemoteNotificationsWithDeviceToken:) method; if registration doesn’t succeed, the delegate is informed via the application(_:didFailToRegisterForRemoteNotificationsWithError:) method. If the app delegate receives a device token, it should connect with its provider and pass it the token.

iOS does not display or play notification types specified in the notification payload that are not one of the requested ones. For example, if alert messages are not one of the accepted notification types, iOS does not display an alert even if one is specified in the notification payload. To find out what the app’s current notification types are, call the enabledRemoteNotificationTypes() method.

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

