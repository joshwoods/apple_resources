

- IOBluetooth
- IOBluetoothDevice
-  init(addressString:) 

Initializer

# init(addressString:)

Returns the IOBluetoothDevice object for the given BluetoothDeviceAddress

macOS

``` source
convenience init!(addressString address: String!)
```

## Parameters 

`address`  

Pointer to an NSString containing the BD_ADDR for which an IOBluetoothDevice instance is desired. The string should be of the form xx:xx:xx:xx:xx:xx

## Return Value

Returns the IOBluetoothDevice object for the given BluetoothDeviceAddress

## Discussion

Within a single application, there will be only one instance of IOBluetoothDevice for a given remote device address.

## See Also

### Initializers

convenience init!(address: UnsafePointer&lt;BluetoothDeviceAddress>!)

Returns the IOBluetoothDevice object for the given BluetoothDeviceAddress

