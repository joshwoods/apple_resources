

- IOBluetooth
- IOBluetoothRFCOMMChannel
-  isIncoming() 

Instance Method

# isIncoming()

Returns the direction of the channel. An incoming channel is one that was opened by the remote device.

macOS

``` source
func isIncoming() -> Bool
```

## Return Value

Returns TRUE if the channel was opened by the remote device, FALSE if the channel was opened by this object.

