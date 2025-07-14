

- IOBluetooth
- IOBluetoothHostController
-  nameAsString() 

Instance Method

# nameAsString()

Gets the “friendly” name of HCI controller.

macOS

``` source
func nameAsString() -> String!
```

## Return Value

Returns NSString with the device name, nil if there is not one or it cannot be read.

