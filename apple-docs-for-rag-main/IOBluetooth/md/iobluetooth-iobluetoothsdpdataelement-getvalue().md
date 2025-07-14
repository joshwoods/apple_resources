

- IOBluetooth
- IOBluetoothSDPDataElement
-  getValue() 

Instance Method

# getValue()

Returns the object value of the data element.

macOS

``` source
func getValue() -> NSObject!
```

## Return Value

Returns the object value of the target data element.

## Discussion

The value returned may be an NSNumber, NSString, NSData, NSArray or IOBluetoothSDPDataElement depending on the type of the data element.

