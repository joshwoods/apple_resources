

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  matchesUUIDArray(\_:) 

Instance Method

# matchesUUIDArray(\_:)

Returns TRUE if ALL of the UUIDs in the given array is found in the target service.

macOS

``` source
func matchesUUIDArray(_ uuidArray: [Any]!) -> Bool
```

## Parameters 

`uuidArray`  

An NSArray of IOBluetoothSDPUUID objects to search for in the target service.

## Return Value

Returns TRUE if all of the given UUIDs are present in the service.

## Discussion

The given array should contain IOBluetoothSDPUUID objects. It only returns TRUE if all of the UUIDs are found. This method is like hasServiceFromArray: except that it requires that all UUIDs match instead of any of them matching.

NOTE: This method is only available in macOS 10.2.4 (Bluetooth v1.1) or later.

