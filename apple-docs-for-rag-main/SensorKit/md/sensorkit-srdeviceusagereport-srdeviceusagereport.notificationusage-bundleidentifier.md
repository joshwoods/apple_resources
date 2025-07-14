

- SensorKit
- SRDeviceUsageReport
- SRDeviceUsageReport.NotificationUsage
-  bundleIdentifier 

Instance Property

# bundleIdentifier

The bundle identifier of the app that corresponds to the notification.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var bundleIdentifier: String? { get }
```

## Discussion

The framework sets a value for this property only if the bundle identifier corresponds to an Apple app.

## See Also

### Analyzing Notification Use

var event: SRDeviceUsageReport.NotificationUsage.Event

The way that the user interacts with the notification.

enum Event

The ways that a user interacts with notifications.

