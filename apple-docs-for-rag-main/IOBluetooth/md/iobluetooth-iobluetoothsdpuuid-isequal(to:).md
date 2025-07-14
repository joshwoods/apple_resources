

- IOBluetooth
- IOBluetoothSDPUUID
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Compares the target IOBluetoothSDPUUID object with the given otherUUID object.

macOS

``` source
func isEqual(to otherUUID: IOBluetoothSDPUUID!) -> Bool
```

## Parameters 

`otherUUID`  

The UUID object to be compared with the target.

## Return Value

Returns true if the UUID values of each object are equal. This includes the case where the sizes are different but the data itself is the same when the Bluetooth UUID base is applied.

## Discussion

This method will compare the two UUID values independent of their length.

