

- UIKit
- UIApplication
-  enabledRemoteNotificationTypes() Deprecated

Instance Method

# enabledRemoteNotificationTypes()

Returns the types of notifications the app accepts.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func enabledRemoteNotificationTypes() -> UIRemoteNotificationType
```

Deprecated

Use the isRegisteredForRemoteNotifications method instead.

## Return Value

A bit mask whose values indicate the types of notifications the user has requested for the app. See UIRemoteNotificationType for valid bit-mask values.

## Discussion

The values in the returned bit mask indicate the types of notifications currently enabled for the app. These types are first set when the app calls the registerForRemoteNotifications(matching:) method to register itself with Apple Push Notification service. Thereafter, the user may modify these accepted notification types in the Notifications preference of the Settings app. This method returns those initial or modified values. iOS does not display or play notification types specified in the notification payload that are not one of the enabled types. For example, the app might accept icon-badging as a form of notification, but might reject sounds and alert messages, even if they are specified in the notification payload.

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

