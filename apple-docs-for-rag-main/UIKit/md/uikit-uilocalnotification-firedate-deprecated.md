

- UIKit
- UILocalNotification
-  fireDate Deprecated

Instance Property

# fireDate

The date and time when the system should deliver the notification.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var fireDate: Date? { get set }
```

## Discussion

The fire date is interpreted according to the value specified in the timeZone property. If the specified value is `nil` or is a date in the past, the notification is delivered immediately.

You may specify a value for this property or the region property but not both. Attempting to schedule a local notification that contains both a region and fire date raises an exception.

## See Also

### Scheduling a local notification

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

var regionTriggersOnce: Bool

A Boolean value indicating whether crossing a geographic region boundary delivers only one notification.

Deprecated

