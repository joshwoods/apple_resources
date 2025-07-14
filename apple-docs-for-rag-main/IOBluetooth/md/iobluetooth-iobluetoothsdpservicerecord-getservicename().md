

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  getServiceName() 

Instance Method

# getServiceName()

Returns the name of the service.

macOS

``` source
func getServiceName() -> String!
```

## Return Value

Returns the name of the target service.

## Discussion

This is currently implemented to simply return the attribute with an id of 0x0100. In the future, it will be extended to allow name localization based on the user’s chosen language or other languages.

