

- Foundation
- NSUserNotification
-  deliveryDate Deprecated

Instance Property

# deliveryDate

Specifies when the notification should be delivered.

macOS 10.8–11.0Deprecated

``` source
var deliveryDate: Date? { get set }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

The delivery date is specified in an absolute time.

After a notification is delivered, it may be presented to the user.

## See Also

### Delivery Timing

var actualDeliveryDate: Date?

The date this notification was actually delivered.

Deprecated

var deliveryRepeatInterval: DateComponents?

Specifies the date components that control how often a user notification is repeated.

Deprecated

var deliveryTimeZone: TimeZone?

Specify the time zone to interpret the delivery date in.

Deprecated

