

- UIKit
- UILocalNotification
-  timeZone Deprecated

Instance Property

# timeZone

The time zone of the notification’s fire date.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var timeZone: TimeZone? { get set }
```

## Discussion

The date specified in fireDate is interpreted according to the value of this property. If you specify `nil` (the default), the fire date is interpreted as an absolute GMT time, which is suitable for cases such as countdown timers. If you assign a valid NSTimeZone object to this property, the fire date is interpreted as a wall-clock time that is automatically adjusted when there are changes in time zones; an example suitable for this case is an an alarm clock.

## See Also

### Scheduling a local notification

var fireDate: Date?

The date and time when the system should deliver the notification.

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

