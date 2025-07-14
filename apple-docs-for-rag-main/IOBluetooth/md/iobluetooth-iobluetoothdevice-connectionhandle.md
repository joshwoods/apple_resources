

- IOBluetooth
- IOBluetoothDevice
-  connectionHandle 

Instance Property

# connectionHandle

Get the connection handle for the baseband connection.

macOS

``` source
var connectionHandle: BluetoothConnectionHandle { get }
```

## Discussion

This method only returns a valid result if a baseband connection is present (-isConnected returns TRUE).

