

- AppKit
- NSApplication
-  isRegisteredForRemoteNotifications 

Instance Property

# isRegisteredForRemoteNotifications

A Boolean value indicating whether the app is registered with Apple Push Notification service (APNs).

macOS 10.14+

``` source
@MainActor
var isRegisteredForRemoteNotifications: Bool { get }
```

## See Also

### Managing Remote Notifications

func registerForRemoteNotifications()

Register for notifications sent by Apple Push Notification service (APNs).

func unregisterForRemoteNotifications()

Unregister for notifications received from Apple Push Notification service.

var enabledRemoteNotificationTypes: NSApplication.RemoteNotificationType

The types of push notifications that the app accepts.

func registerForRemoteNotifications(matching: NSApplication.RemoteNotificationType)

Register to receive notifications of the specified types from a provider through the Apple Push Notification service.

Deprecated

struct RemoteNotificationType

These constants determine whether apps launched by remote notifications display a badge.

