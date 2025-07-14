

- IOBluetooth
- IOBluetoothSDPDataElement
-  getArrayValue() 

Instance Method

# getArrayValue()

If the data element is represented by an array object, it returns the value as an NSArray.

macOS

``` source
func getArrayValue() -> [Any]!
```

## Return Value

Returns an NSArray representation of the data element if it is a sequence type.

## Discussion

The data types represented by an array object are 6 (data element sequence) and 7 (data element alternative).

