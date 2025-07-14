

- IOBluetooth
- IOBluetoothRFCOMMChannel
-  register(forChannelCloseNotification:selector:) 

Instance Method

# register(forChannelCloseNotification:selector:)

Allows a client to register for a channel close notification.

macOS

``` source
func register(
    forChannelCloseNotification observer: Any!,
    selector inSelector: Selector!
) -> IOBluetoothUserNotification!
```

## Parameters 

`observer`  

Target observer object

`inSelector`  

Selector to be sent to the observer when the RFCOMM channel is closed.

## Return Value

Returns an IOBluetoothUserNotification representing the outstanding RFCOMM channel close notification. To unregister the notification, call -unregister of the returned IOBluetoothUserNotification object. If an error is encountered creating the notification, nil is returned.

## Discussion

The given selector will be called on the target observer when the RFCOMM channel is closed. The selector should contain two arguments. The first is the user notification object. The second is the IOBluetoothRFCOMMChannel that was closed.

