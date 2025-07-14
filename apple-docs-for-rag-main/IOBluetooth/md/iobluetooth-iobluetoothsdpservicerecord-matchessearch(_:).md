

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  matchesSearch(\_:) 

Instance Method

# matchesSearch(\_:)

Returns TRUE any of the UUID arrays in the search array match the target service.

macOS

``` source
func matchesSearch(_ searchArray: [Any]!) -> Bool
```

## Parameters 

`searchArray`  

An NSArray of NSArrays of IOBluetoothSDPUUID objects.

## Return Value

Returns `TRUE` if any of the UUID arrays match.

## Discussion

The given array should contain NSArray objects. Each sub-NSArray should contain IOBluetoothSDPUUID objects. In turn, each sub-NSArray gets passed to -matchesUUIDArray: If any of those returns `TRUE`, then the search stops and `TRUE` is returned. Essentially the primary NSArray contains the OR operations and each sub-array contains the AND operations.

NOTE: This method is only available in macOS 10.2.4 (Bluetooth v1.1) or later.

