

- AppKit
- NSApplication
-  NSApplication.RemoteNotificationType 

Structure

# NSApplication.RemoteNotificationType

These constants determine whether apps launched by remote notifications display a badge.

macOS

``` source
struct RemoteNotificationType
```

## Topics

### Interaction Types

static var badge: NSApplication.RemoteNotificationType

The app should display a badge.

static var sound: NSApplication.RemoteNotificationType

The app should play a sound.

static var alert: NSApplication.RemoteNotificationType

The app should display an alert.

### Initializers

init(rawValue: UInt)

Initializes a new remote notifications options structure.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

var isRegisteredForRemoteNotifications: Bool

A Boolean value indicating whether the app is registered with Apple Push Notification service (APNs).

