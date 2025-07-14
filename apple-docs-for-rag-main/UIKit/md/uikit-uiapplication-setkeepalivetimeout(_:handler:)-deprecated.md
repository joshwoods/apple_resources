

- UIKit
- UIApplication
-  setKeepAliveTimeout(\_:handler:) Deprecated

Instance Method

# setKeepAliveTimeout(\_:handler:)

Configures a periodic handler for VoIP apps in older versions of iOS.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func setKeepAliveTimeout(
    _ timeout: TimeInterval,
    handler keepAliveHandler: (() -> Void)? = nil
) -> Bool
```

Deprecated

This legacy VoIP API was deprecated in iOS 10.0. Use PushKit to develop VoIP apps.

## Parameters 

`timeout`  

The maximum interval (measured in seconds) at which your app should be woken up to check its VoIP connection. The minimum acceptable timeout value is 600 seconds.

`keepAliveHandler`  

A block that performs the tasks needed to maintain your VoIP network connection. Setting this parameter to `nil` releases the current handler block and prevents UIKit from scheduling the next wake.

## Return Value

true if the handler was installed or false if it was not.

## Discussion

In iOS 8 and later, voice-over-IP (VoIP) apps register for registerForRemoteNotifications() remote notifications instead of using this method. Using remote notifications eliminates the need for a timeout handler to check in with the VoIP service. Instead, when a calls arrives for the user, the VoIP service sends a VoIP remote notification to the user’s device. Upon receiving this notification, the device launches or wakes the app as needed so that it can handle the incoming call.

In iOS 7 and earlier, VoIP apps use this method to install a handler whose job is to maintain the app’s network connection with a VoIP server. This handler is guaranteed to be called before the specified timeout value but may be called at a slightly different time interval in order to better align execution of your handler with other system tasks, and thereby save power. Your handler has a maximum of 10 seconds to perform any needed tasks and exit. If it does not exit before time expires, the app is suspended.

Timeout values and handlers are not persisted between app launches. Therefore, if your app is terminated for any reason, you must reinstall the handler during the next launch cycle.

For calls to this method to succeed, the app must have the `voip` value in the array associated with the `UIBackgroundModes` key in its `Info.plist` file. Calling this method replaces the previously installed handler and timeout values, if any.

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

