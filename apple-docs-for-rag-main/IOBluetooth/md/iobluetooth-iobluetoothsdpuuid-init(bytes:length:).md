

- IOBluetooth
- IOBluetoothSDPUUID
-  init(bytes:length:) 

Initializer

# init(bytes:length:)

Creates a new IOBluetoothSDPUUID object with the given bytes of the given length.

macOS

``` source
convenience init!(
    bytes: UnsafeRawPointer!,
    length: UInt32
)
```

## Parameters 

`bytes`  

An array of bytes representing the UUID.

`length`  

The length of the array of bytes.

## Return Value

Returns the new IOBluetoothSDPUUID object or nil on failure.

## Discussion

If the length is invalid for a UUID, nil is returned.

## See Also

### Initializers

convenience init!(data: Data!)

Creates a new IOBluetoothSDPUUID object from the given NSData.

init!(uuid16: BluetoothSDPUUID16)

Initializes a new 16-bit IOBluetoothSDPUUID with the given UUID16

init!(uuid32: BluetoothSDPUUID32)

Creates a new 32-bit IOBluetoothSDPUUID with the given UUID32

