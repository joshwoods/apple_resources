

- AppKit
- NSApplication
-  unregisterForRemoteNotifications() 

Instance Method

# unregisterForRemoteNotifications()

Unregister for notifications received from Apple Push Notification service.

macOS 10.7+

``` source
@MainActor
func unregisterForRemoteNotifications()
```

## Discussion

You should only call this method in rare circumstances, such as when a new version of the app drops support for remote notifications. Apps unregistered through this method can always reregister.

## See Also

### Managing Remote Notifications

func registerForRemoteNotifications()

Register for notifications sent by Apple Push Notification service (APNs).

var enabledRemoteNotificationTypes: NSApplication.RemoteNotificationType

The types of push notifications that the app accepts.

func registerForRemoteNotifications(matching: NSApplication.RemoteNotificationType)

Register to receive notifications of the specified types from a provider through the Apple Push Notification service.

Deprecated

var isRegisteredForRemoteNotifications: Bool

A Boolean value indicating whether the app is registered with Apple Push Notification service (APNs).

struct RemoteNotificationType

These constants determine whether apps launched by remote notifications display a badge.

