

- Foundation
- NSUserNotification
-  actualDeliveryDate Deprecated

Instance Property

# actualDeliveryDate

The date this notification was actually delivered.

macOS 10.8–11.0Deprecated

``` source
var actualDeliveryDate: Date? { get }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

The notification center will set this value if a notification is put in the scheduled list and the delivery time arrives.

If the notification is delivered directly using the deliver(_:) method of the NSUserNotificationCenter class, this value is set to the deliveryDate value. If the deliveryDate value `nil` this value is set to the current date.

This value is used to sort the list of notifications in the user interface.

## See Also

### Delivery Timing

var deliveryDate: Date?

Specifies when the notification should be delivered.

Deprecated

var deliveryRepeatInterval: DateComponents?

Specifies the date components that control how often a user notification is repeated.

Deprecated

var deliveryTimeZone: TimeZone?

Specify the time zone to interpret the delivery date in.

Deprecated

