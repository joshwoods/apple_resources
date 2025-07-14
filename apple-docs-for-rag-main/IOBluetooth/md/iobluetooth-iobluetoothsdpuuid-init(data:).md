

- IOBluetooth
- IOBluetoothSDPUUID
-  init(data:) 

Initializer

# init(data:)

Creates a new IOBluetoothSDPUUID object from the given NSData.

macOS

``` source
convenience init!(data: Data!)
```

## Parameters 

`data`  

The NSData containing the UUID bytes.

## Return Value

Returns the new IOBluetoothSDPUUID object or nil on failure.

## Discussion

If the length of the NSData is invalid for a UUID, nil is returned.

## See Also

### Initializers

convenience init!(bytes: UnsafeRawPointer!, length: UInt32)

Creates a new IOBluetoothSDPUUID object with the given bytes of the given length.

init!(uuid16: BluetoothSDPUUID16)

Initializes a new 16-bit IOBluetoothSDPUUID with the given UUID16

init!(uuid32: BluetoothSDPUUID32)

Creates a new 32-bit IOBluetoothSDPUUID with the given UUID32

