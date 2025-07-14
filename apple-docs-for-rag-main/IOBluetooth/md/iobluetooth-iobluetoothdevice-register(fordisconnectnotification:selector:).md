

- IOBluetooth
- IOBluetoothDevice
-  register(forDisconnectNotification:selector:) 

Instance Method

# register(forDisconnectNotification:selector:)

Allows a client to register for device disconnect notification.

macOS

``` source
func register(
    forDisconnectNotification observer: Any!,
    selector inSelector: Selector!
) -> IOBluetoothUserNotification!
```

## Parameters 

`observer`  

Target observer object

`inSelector`  

Selector to be sent to the observer when the connection is destroyed

## Return Value

Returns an IOBluetoothUserNotification representing the outstanding device disconnect notification. To unregister the notification, call -unregister of the returned IOBluetoothUserNotification object. If an error is encountered creating the notification, nil is returned.

## Discussion

The given selector will be called on the target observer when the target device’s connection is closed. The selector should contain two arguments. The first is the user notification object. The second is the IOBluetoothDevice that was disconnected.

