

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  hasService(from:) 

Instance Method

# hasService(from:)

Returns TRUE if any one of the UUIDs in the given array is found in the target service.

macOS

``` source
func hasService(from array: [Any]!) -> Bool
```

## Parameters 

`array`  

An NSArray of IOBluetoothSDPUUID objects to search for in the target service.

## Return Value

Returns TRUE if any of the given UUIDs are present in the service.

## Discussion

The given array should contain IOBluetoothSDPUUID objects. It is currently implemented such that it returns TRUE if any of the UUIDs are found. However in the future, it is likely that this will change to more closely match the functionality in the SDP spec so that it only returns TRUE if all of the given UUIDs are present. That way, both AND and OR comparisons can be implemented. Please make a note of this potential change.

