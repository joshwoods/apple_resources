

- AppKit
- NSApplication
-  enabledRemoteNotificationTypes 

Instance Property

# enabledRemoteNotificationTypes

The types of push notifications that the app accepts.

macOS 10.7+

``` source
@MainActor
var enabledRemoteNotificationTypes: NSApplication.RemoteNotificationType { get }
```

## Return Value

A bit mask whose values indicate the types of notifications the user has requested for the app. See NSApplication.RemoteNotificationType for valid bit-mask values.

## Discussion

This property contains a bitmask whose values indicate the types of push notifications that the app requested. You don’t set this property directly. Call the registerForRemoteNotifications(matching:) method to register your app with Apple Push Notification Service and request the notification types your app supports. macOS delivers only notifications of types that the app supports. For a list of possible values, see NSApplication.RemoteNotificationType.

Note

Currently the only notification type supported for non-running apps is the badging of app icons.

## See Also

### Managing Remote Notifications

func registerForRemoteNotifications()

Register for notifications sent by Apple Push Notification service (APNs).

func unregisterForRemoteNotifications()

Unregister for notifications received from Apple Push Notification service.

func registerForRemoteNotifications(matching: NSApplication.RemoteNotificationType)

Register to receive notifications of the specified types from a provider through the Apple Push Notification service.

Deprecated

var isRegisteredForRemoteNotifications: Bool

A Boolean value indicating whether the app is registered with Apple Push Notification service (APNs).

struct RemoteNotificationType

These constants determine whether apps launched by remote notifications display a badge.

