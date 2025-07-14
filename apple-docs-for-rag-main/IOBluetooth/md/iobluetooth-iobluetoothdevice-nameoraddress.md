

- IOBluetooth
- IOBluetoothDevice
-  nameOrAddress 

Instance Property

# nameOrAddress

Get the human readable name of the remote device. If the name is not present, it will return a string containing the device’s address.

macOS

``` source
var nameOrAddress: String! { get }
```

## Discussion

If a remote name request has been successfully completed, the device name will be returned. If not, a string containg the device address in the format of “XX-XX-XX-XX-XX-XX” will be returned.

