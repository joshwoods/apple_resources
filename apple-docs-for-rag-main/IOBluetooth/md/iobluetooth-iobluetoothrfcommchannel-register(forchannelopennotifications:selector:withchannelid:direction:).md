

- IOBluetooth
- IOBluetoothRFCOMMChannel
-  register(forChannelOpenNotifications:selector:withChannelID:direction:) 

Type Method

# register(forChannelOpenNotifications:selector:withChannelID:direction:)

Allows a client to register for RFCOMM channel open notifications for certain types of RFCOMM channels.

macOS

``` source
class func register(
    forChannelOpenNotifications object: Any!,
    selector: Selector!,
    withChannelID channelID: BluetoothRFCOMMChannelID,
    direction inDirection: IOBluetoothUserNotificationChannelDirection
) -> IOBluetoothUserNotification!
```

## Parameters 

`object`  

Target object

`selector`  

Selector to be called on the target object when a new RFCOMM channel is opened. the format for the selector is: -(void) selectorName:(IOBluetoothUserNotification \*)inNotification channel:(IOBluetoothRFCOMMChannel \*)newChannel

`channelID`  

RFCOMM channel ID to match a new RFCOMM channel. If the channel ID doesn’t matter, 0 may be passed in.

`inDirection`  

The desired direction of the RFCOMM channel - kIOBluetoothUserNotificationChannelDirectionAny if the direction doesn’t matter.

## Discussion

The given selector will be called on the target object whenever an RFCOMM channel with the given attributes is opened. The selector should accept two arguments. The first is the user notification object. The second is the IOBluetoothRFCOMMChannel that was opened.

