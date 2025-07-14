

- Foundation
- NSNotification
- NSNotification.Name
-  EAAccessoryDidConnect 

Type Property

# EAAccessoryDidConnect

A notification that the system sends when an accessory becomes connected and available for your application to use.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
static let EAAccessoryDidConnect: NSNotification.Name
```

## Discussion

The notification object is the shared accessory manager. The `userInfo` dictionary contains an EAAccessoryKey, whose value is an EAAccessory object representing the accessory that is now connected. If a Bluetooth accessory was selected by the user in the Bluetooth picker, this dictionary contains the EAAccessorySelectedKey key. Before delivery of this notification can occur, you must call the registerForLocalNotifications() method to let the system know you are interested in receiving this notification.

After receiving this notification, always check the protocolStrings array of the newly connected accessory object to verify that the required protocol is present before trying to open a session. In some cases, the system may send the connection notification before authentication has completed, resulting in an empty protocolStrings array and a subsequent disconnection message. If this happens, the system sends another connection message later, when authentication succeeds.

Important

iPhone and iPad apps running on Macs with Apple silicon never receive this notification.

## See Also

### External Accessory

static let EAAccessoryDidDisconnect: NSNotification.Name

A notification that is posted when an accessory is disconnected and no longer available for your application to use.

