

- Foundation
- NSNotification
- NSNotification.Name
-  EAAccessoryDidDisconnect 

Type Property

# EAAccessoryDidDisconnect

A notification that is posted when an accessory is disconnected and no longer available for your application to use.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
static let EAAccessoryDidDisconnect: NSNotification.Name
```

## Discussion

The notification object is the shared accessory manager. The `userInfo` dictionary contains an EAAccessoryKey, whose value is the EAAccessory object representing the accessory that was disconnected. Before delivery of this notification can occur, you must call the registerForLocalNotifications() method to let the system know you are interested in receiving this notification.

If your accessory manager has a delegate, the delegate can use the accessoryDidDisconnect(_:) method to receive this notification instead.

## See Also

### External Accessory

static let EAAccessoryDidConnect: NSNotification.Name

A notification that the system sends when an accessory becomes connected and available for your application to use.

