

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  init(serviceDictionary:device:) 

Initializer

# init(serviceDictionary:device:)

Returns an initialized IOBluetoothSDPServiceRecord \* with the attributes specified in the provided service dictionary. Provide a pointer to an IOBlueotothDevice if you wish to associate the record to a specific IOBluetoothDevice.

macOS

``` source
init!(
    serviceDictionary serviceDict: [AnyHashable : Any]!,
    device: IOBluetoothDevice!
)
```

