

- IOBluetooth
- IOBluetoothL2CAPChannel
-  objectID 

Instance Property

# objectID

Returns the IOBluetoothObjectID of the given IOBluetoothL2CAPChannel.

macOS

``` source
var objectID: IOBluetoothObjectID { get }
```

## Discussion

The IOBluetoothObjectID can be used as a global reference for a given IOBluetoothL2CAPChannel. It allows two separate applications to refer to the same IOBluetoothL2CAPChannel.

