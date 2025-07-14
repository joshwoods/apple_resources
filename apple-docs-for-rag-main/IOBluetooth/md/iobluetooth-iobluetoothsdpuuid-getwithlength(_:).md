

- IOBluetooth
- IOBluetoothSDPUUID
-  getWithLength(\_:) 

Instance Method

# getWithLength(\_:)

Returns an IOBluetoothSDPUUID object matching the target UUID, but with the given number of bytes.

macOS

``` source
func getWithLength(_ newLength: UInt32) -> Self!
```

## Parameters 

`newLength`  

The desired length for the UUID.

## Return Value

Returns an IOBluetoothSDPUUID object with the same data as the target but with the given length if it is possible to do so. Otherwise, nil is returned.

## Discussion

If the target object is the same length as newLength, it returns self. If newLength is greater it creates a new IOBluetoothSDPUUID object with the correct value for the given length. If newLength is smaller, it will attempt to create a new IOBluetoothSDPUUID that is smaller if the data matches the Bluetooth UUID base. This downconversion is currently unimplemented.

