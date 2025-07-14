

- IOBluetooth
- IOBluetoothSDPDataElement
-  getStringValue() 

Instance Method

# getStringValue()

If the data element is represented by a string object, it returns the value as an NSString.

macOS

``` source
func getStringValue() -> String!
```

## Return Value

Returns an NSString representation of the data element if it is a text or URL type.

## Discussion

The data types represented by a string object are 4 (text string) and 8 (URL).

