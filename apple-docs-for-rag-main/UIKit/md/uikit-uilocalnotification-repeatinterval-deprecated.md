

- UIKit
- UILocalNotification
-  repeatInterval Deprecated

Instance Property

# repeatInterval

The calendar interval at which to reschedule the notification.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var repeatInterval: NSCalendar.Unit { get set }
```

## Discussion

If you assign a calendar unit such as weekly (weekOfYear) or yearly (year), the system reschedules the notification for delivery at the specified interval. Note that intervals of less than one minute are not supported. The default value is 0, which means that the system fires the notification once and then discards it.

## See Also

### Scheduling a local notification

var fireDate: Date?

The date and time when the system should deliver the notification.

Deprecated

var timeZone: TimeZone?

The time zone of the notification’s fire date.

Deprecated

var repeatCalendar: Calendar?

The calendar the system should refer to when it reschedules a repeating notification.

Deprecated

var region: CLRegion?

The geographic region that triggers the notification.

Deprecated

var regionTriggersOnce: Bool

A Boolean value indicating whether crossing a geographic region boundary delivers only one notification.

Deprecated

