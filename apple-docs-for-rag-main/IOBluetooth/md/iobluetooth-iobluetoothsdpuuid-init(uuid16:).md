

- IOBluetooth
- IOBluetoothSDPUUID
-  init(uuid16:) 

Initializer

# init(uuid16:)

Initializes a new 16-bit IOBluetoothSDPUUID with the given UUID16

macOS

``` source
init!(uuid16: BluetoothSDPUUID16)
```

## Parameters 

`uuid16`  

A scalar representing a 16-bit UUID

## Return Value

Returns self.

## See Also

### Initializers

convenience init!(bytes: UnsafeRawPointer!, length: UInt32)

Creates a new IOBluetoothSDPUUID object with the given bytes of the given length.

convenience init!(data: Data!)

Creates a new IOBluetoothSDPUUID object from the given NSData.

init!(uuid32: BluetoothSDPUUID32)

Creates a new 32-bit IOBluetoothSDPUUID with the given UUID32

