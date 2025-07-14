

- IOBluetooth
- IOBluetoothSDPDataElement
-  getDataValue() 

Instance Method

# getDataValue()

If the data element is represented by a data object, it returns the value as an NSData.

macOS

``` source
func getDataValue() -> Data!
```

## Return Value

Returns an NSData representation of the data element if it is a 128-bit number.

## Discussion

The data types represented by a data object are 128-bit versions of 1 (unsigned int) and 2 (signed int).

