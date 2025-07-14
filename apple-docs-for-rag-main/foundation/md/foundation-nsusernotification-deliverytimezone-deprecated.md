

- Foundation
- NSUserNotification
-  deliveryTimeZone Deprecated

Instance Property

# deliveryTimeZone

Specify the time zone to interpret the delivery date in.

macOS 10.8–11.0Deprecated

``` source
var deliveryTimeZone: TimeZone? { get set }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

If this value is `nil` and the user switches time zones, the notification center will adjust the time of presentation to account for the time zone change.

If a notification should be delivered at a time in a specific time zone (regardless of whether the user switches time zones), set this value to the specific time zone, for example the current time zone.

## See Also

### Delivery Timing

var deliveryDate: Date?

Specifies when the notification should be delivered.

Deprecated

var actualDeliveryDate: Date?

The date this notification was actually delivered.

Deprecated

var deliveryRepeatInterval: DateComponents?

Specifies the date components that control how often a user notification is repeated.

Deprecated

