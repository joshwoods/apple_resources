

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  device 

Instance Property

# device

Returns the IOBluetoothDevice that the target service belongs to.

macOS

``` source
var device: IOBluetoothDevice! { get }
```

## Return Value

Returns the IOBluetoothDevice that the target service belongs to. If the service is one the local host is vending, then nil is returned.

## Discussion

If the service is a local service (i.e. one the current host is vending out), then nil is returned.

