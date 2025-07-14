

- Foundation
- NSUserNotification
-  deliveryRepeatInterval Deprecated

Instance Property

# deliveryRepeatInterval

Specifies the date components that control how often a user notification is repeated.

macOS 10.8–11.0Deprecated

``` source
var deliveryRepeatInterval: DateComponents? { get set }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

This value may be `nil` if the notification should not repeat.

The date component values are relative to the date the notification was delivered.

If the calendar value of the `deliveryRepeatInterval` is `nil`, the current calendar is used to calculate the repeat interval. For example, if a notification should repeat every hour, set the `hour` property of the `deliveryRepeatInterval` to `1`.

This value is ignored unless the user notification is scheduled with the NSUserNotificationCenter object.

## See Also

### Delivery Timing

var deliveryDate: Date?

Specifies when the notification should be delivered.

Deprecated

var actualDeliveryDate: Date?

The date this notification was actually delivered.

Deprecated

var deliveryTimeZone: TimeZone?

Specify the time zone to interpret the delivery date in.

Deprecated

