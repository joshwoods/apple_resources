

- IOBluetooth
- IOBluetoothDevice
-  init(address:) 

Initializer

# init(address:)

Returns the IOBluetoothDevice object for the given BluetoothDeviceAddress

macOS

``` source
convenience init!(address: UnsafePointer!)
```

## Parameters 

`address`  

Pointer to a BluetoothDeviceAddress for which an IOBluetoothDevice instance is desired

## Return Value

Returns the IOBluetoothDevice object for the given BluetoothDeviceAddress

## Discussion

Within a single application, there will be only one instance of IOBluetoothDevice for a given remote device address.

## See Also

### Initializers

convenience init!(addressString: String!)

Returns the IOBluetoothDevice object for the given BluetoothDeviceAddress

