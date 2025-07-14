

- AppKit
- NSApplication
-  registerForRemoteNotifications(matching:) Deprecated

Instance Method

# registerForRemoteNotifications(matching:)

Register to receive notifications of the specified types from a provider through the Apple Push Notification service.

macOS 10.7+

``` source
@MainActor
func registerForRemoteNotifications(matching types: NSApplication.RemoteNotificationType)
```

Deprecated

Use registerForRemoteNotifications() instead.

## Parameters 

`types`  

A bit mask specifying the types of notifications the app accepts. See NSApplication.RemoteNotificationType for valid bit-mask values.

## Discussion

When you send this message, the device initiates the registration process with Apple Push Notification Service. If it succeeds, the app delegate receives a device token in the application(_:didRegisterForRemoteNotificationsWithDeviceToken:) method; if registration doesn’t succeed, the delegate is informed via the application(_:didFailToRegisterForRemoteNotificationsWithError:) method. If the app delegate receives a device token, it should connect with its provider and pass it the token.

Note

Currently the only notification type supported in macOS for non-running apps is icon badging. However, the JSON payload, which may contain information related to sounds and alerts, is passed to a running app in application(_:didReceiveRemoteNotification:). The app can do whatever it wants to with that information (for example, display an alert or play a sound).

## See Also

### Managing Remote Notifications

func registerForRemoteNotifications()

Register for notifications sent by Apple Push Notification service (APNs).

func unregisterForRemoteNotifications()

Unregister for notifications received from Apple Push Notification service.

var enabledRemoteNotificationTypes: NSApplication.RemoteNotificationType

The types of push notifications that the app accepts.

var isRegisteredForRemoteNotifications: Bool

A Boolean value indicating whether the app is registered with Apple Push Notification service (APNs).

struct RemoteNotificationType

These constants determine whether apps launched by remote notifications display a badge.

