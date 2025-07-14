

- UIKit
- UILocalNotification
-  regionTriggersOnce Deprecated

Instance Property

# regionTriggersOnce

A Boolean value indicating whether crossing a geographic region boundary delivers only one notification.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var regionTriggersOnce: Bool { get set }
```

## Discussion

When the value of this property is true, the user is notified only upon the first crossing the boundary of the target region. After the first crossing, the local notification is unscheduled. When the value of this property is false, notifications are delivered with each boundary crossing. The default value of this property is true.

The region object itself defines whether the notification is triggered when the user enters or exits the region.

## See Also

### Scheduling a local notification

var fireDate: Date?

The date and time when the system should deliver the notification.

Deprecated

var timeZone: TimeZone?

The time zone of the notification’s fire date.

Deprecated

var repeatInterval: NSCalendar.Unit

The calendar interval at which to reschedule the notification.

Deprecated

var repeatCalendar: Calendar?

The calendar the system should refer to when it reschedules a repeating notification.

Deprecated

var region: CLRegion?

The geographic region that triggers the notification.

Deprecated

