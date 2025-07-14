

- IOBluetooth
- IOBluetoothSDPDataElement
-  getUUIDValue() 

Instance Method

# getUUIDValue()

If the data element is a UUID (type 3), it returns the value as an IOBluetoothSDPUUID.

macOS

``` source
func getUUIDValue() -> IOBluetoothSDPUUID!
```

## Return Value

Returns an IOBluetoothSDPUUID representation of the data element if it is a UUID.

