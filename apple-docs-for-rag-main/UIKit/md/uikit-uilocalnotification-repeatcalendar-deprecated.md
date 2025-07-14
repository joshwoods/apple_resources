

- UIKit
- UILocalNotification
-  repeatCalendar Deprecated

Instance Property

# repeatCalendar

The calendar the system should refer to when it reschedules a repeating notification.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedwatchOS 2.0–3.0Deprecated

``` source
@MainActor
var repeatCalendar: Calendar? { get set }
```

## Discussion

The default value is `nil`, which indicates that the current user calendar is used. (The current user calendar is returned by the current class method of `NSCalendar`.)

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

var region: CLRegion?

The geographic region that triggers the notification.

Deprecated

var regionTriggersOnce: Bool

A Boolean value indicating whether crossing a geographic region boundary delivers only one notification.

Deprecated

