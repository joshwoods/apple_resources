

- IOBluetooth
- IOBluetoothDevice
-  name 

Instance Property

# name

Get the human readable name of the remote device.

macOS

``` source
var name: String! { get }
```

## Discussion

This only returns a value if a remote name request has been performed on the target device. If a successful remote name request has not been completed, nil is returned. To perform a remote name request, call -remoteNameRequest. If a remote name request has been successfully completed, the method -getLastNameUpdate will return the date/time of the last successful request.

