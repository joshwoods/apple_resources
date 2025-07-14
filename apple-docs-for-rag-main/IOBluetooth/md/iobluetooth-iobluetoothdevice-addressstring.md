

- IOBluetooth
- IOBluetoothDevice
-  addressString 

Instance Property

# addressString

Get a string representation of the Bluetooth device address for the target device. The format of the string is the same as returned by IOBluetoothNSStringFromDeviceAddress().

macOS

``` source
var addressString: String! { get }
```

## Discussion

NOTE: This method is only available in macOS 10.2.4 (Bluetooth v1.1) or later.

