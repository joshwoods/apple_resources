

- IOBluetooth
- IOBluetoothDevice
-  getLinkType() 

Instance Method

# getLinkType()

Get the link type for the baseband connection.

macOS

``` source
func getLinkType() -> BluetoothLinkType
```

## Return Value

Returns the link type for the baseband connection. If no baseband connection is present, kBluetoothLinkTypeNone is returned.

## Discussion

This method only returns a valid result if a baseband connection is present (-isConnected returns TRUE).

