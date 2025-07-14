

- UIKit
- UIApplication
-  requestSceneSessionActivation(\_:userActivity:options:errorHandler:) Deprecated

Instance Method

# requestSceneSessionActivation(\_:userActivity:options:errorHandler:)

Asks the system to activate an existing scene, or create a new scene and associate it with your app.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.1+tvOS 13.0+visionOS 1.0–2.4Deprecated

``` source
@MainActor
func requestSceneSessionActivation(
    _ sceneSession: UISceneSession?,
    userActivity: NSUserActivity?,
    options: UIScene.ActivationRequestOptions?,
    errorHandler: ((any Error) -> Void)? = nil
)
```

Deprecated

Use activateSceneSession(for:errorHandler:) (Swift) or activateSceneSessionForRequest:errorHandler: (Objective-C) instead.

## Parameters 

`sceneSession`  

The session whose scene you want to activate. Specify `nil` when you want the system to create a new scene for your app.

`userActivity`  

A user activity object to dispatch to the session’s scene. Use this object to communicate details about a task you want the scene to perform.

`options`  

Information for the system to use when creating or activating the scene. For information about how to create this object, see UIScene.ActivationRequestOptions.

`errorHandler`  

An error handler block to execute if a problem occurs. The method doesn’t execute this block when it successfully activates the scene. This block has no return value and has the following parameter:

error  
The NSError object describing the problem that occurred.

## Discussion

Call this method when you want the system to display one of your app’s scenes. For example, you might call this method to dispatch work to the scene in the form of an NSUserActivity object. When activating an existing session whose scene is no longer in memory, the system creates a new scene and connects it to your app. Similarly, specifying `nil` for the `sceneSession` parameter causes the system to create a new scene and corresponding session.

## See Also

### Deprecated methods

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

func registerForRemoteNotifications(matching: UIRemoteNotificationType)

Register to receive remote notifications of the specified types via Apple Push Notification service.

Deprecated

