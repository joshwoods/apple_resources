

- SensorKit
- SRDeviceUsageReport
- SRDeviceUsageReport.NotificationUsage
-  SRDeviceUsageReport.NotificationUsage.Event 

Enumeration

# SRDeviceUsageReport.NotificationUsage.Event

The ways that a user interacts with notifications.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum Event
```

## Topics

### Events

case appLaunch

A notification of an app launch.

case bannerPulldown

A notification of a banner pull down.

case clear

A notification of a clear event.

case deduped

A notification of a deduped event.

case defaultAction

A notification of a default action.

case deviceActivated

A notification of device activation.

case deviceUnlocked

A notification of a device unlock.

case expired

A notification of an expiration event.

case hide

A notification of a hide event.

case longLook

A notification of a long look.

case notificationCenterClearAll

A notification of clear-all event.

case received

A notification of a received event.

case removed

A notification of a removed event.

case silence

A notification of a silence event.

case supplementaryAction

A notification of a supplementary action.

case tapCoalesce

A notification of a tap-coalesce event.

case unknown

A notification of an unknown event.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Analyzing Notification Use

var bundleIdentifier: String?

The bundle identifier of the app that corresponds to the notification.

var event: SRDeviceUsageReport.NotificationUsage.Event

The way that the user interacts with the notification.

