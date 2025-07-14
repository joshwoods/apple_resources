

- IOBluetooth
- IOBluetoothDevice
-  getLastServicesUpdate() 

Instance Method

# getLastServicesUpdate()

Get the date/time of the last SDP query.

macOS

``` source
func getLastServicesUpdate() -> Date!
```

## Return Value

Returns the date/time of the last SDP query. If an SDP query has never been performed on the device, nil is returned.

