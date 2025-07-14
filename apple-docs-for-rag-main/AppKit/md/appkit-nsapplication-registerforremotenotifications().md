

- AppKit
- NSApplication
-  registerForRemoteNotifications() 

Instance Method

# registerForRemoteNotifications()

Register for notifications sent by Apple Push Notification service (APNs).

macOS 10.14+

``` source
@MainActor
func registerForRemoteNotifications()
```

## Discussion

Call this method to register your app with APNs. When a valid connection is established, APNs sends a device token to your app delegate. Forward that token to your company’s provider server.

For more information about how to register with APNs, see Registering your app with APNs.

## See Also

### Managing Remote Notifications

func unregisterForRemoteNotifications()

Unregister for notifications received from Apple Push Notification service.

var enabledRemoteNotificationTypes: NSApplication.RemoteNotificationType

The types of push notifications that the app accepts.

func registerForRemoteNotifications(matching: NSApplication.RemoteNotificationType)

Register to receive notifications of the specified types from a provider through the Apple Push Notification service.

Deprecated

var isRegisteredForRemoteNotifications: Bool

A Boolean value indicating whether the app is registered with Apple Push Notification service (APNs).

struct RemoteNotificationType

These constants determine whether apps launched by remote notifications display a badge.

