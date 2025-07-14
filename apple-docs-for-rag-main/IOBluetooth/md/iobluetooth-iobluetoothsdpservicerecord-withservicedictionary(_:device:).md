

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  withServiceDictionary(\_:device:) 

Type Method

# withServiceDictionary(\_:device:)

Returns an IOBluetoothSDPServiceRecord \* with the attributes specified in the provided service dictionary. Provide a pointer to an IOBlueotothDevice if you wish to associate the record to a specific IOBluetoothDevice.

macOS

``` source
class func withServiceDictionary(
    _ serviceDict: [AnyHashable : Any]!,
    device: IOBluetoothDevice!
) -> Self!
```

## Return Value

Returns an IOBluetoothSDPServiceRecord \* with the attributes specified in the provided dictionary.

