

- IOBluetooth
- IOBluetoothRFCOMMChannel
-  getObjectID() 

Instance Method

# getObjectID()

Returns the IOBluetoothObjectID of the given IOBluetoothRFCOMMChannel.

macOS

``` source
func getObjectID() -> IOBluetoothObjectID
```

## Return Value

Returns the IOBluetoothObjectID of the given IOBluetoothRFCOMMChannel.

## Discussion

The IOBluetoothObjectID can be used as a global reference for a given IOBluetoothRFCOMMChannel. It allows two separate applications to refer to the same IOBluetoothRFCOMMChannel.

