

- IOBluetooth
- IOBluetoothSDPUUID
-  init(uuid32:) 

Initializer

# init(uuid32:)

Creates a new 32-bit IOBluetoothSDPUUID with the given UUID32

macOS

``` source
init!(uuid32: BluetoothSDPUUID32)
```

## Parameters 

`uuid32`  

A scalar representing a 32-bit UUID

## Return Value

Returns self.

## See Also

### Initializers

convenience init!(bytes: UnsafeRawPointer!, length: UInt32)

Creates a new IOBluetoothSDPUUID object with the given bytes of the given length.

convenience init!(data: Data!)

Creates a new IOBluetoothSDPUUID object from the given NSData.

init!(uuid16: BluetoothSDPUUID16)

Initializes a new 16-bit IOBluetoothSDPUUID with the given UUID16

