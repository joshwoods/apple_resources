

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  matchesUUID16(\_:) 

Instance Method

# matchesUUID16(\_:)

Returns TRUE the UUID16 is found in the target service.

macOS

``` source
func matchesUUID16(_ uuid16: BluetoothSDPUUID16) -> Bool
```

## Parameters 

`uuid16`  

A BluetoothSDPUUID16 to search for in the target service.

## Return Value

Returns TRUE if the UUID16 is present in the service.

## Discussion

NOTE: This method is only available in macOS 10.7 or later.

