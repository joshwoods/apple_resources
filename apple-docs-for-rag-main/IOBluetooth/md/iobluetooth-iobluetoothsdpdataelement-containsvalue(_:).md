

- IOBluetooth
- IOBluetoothSDPDataElement
-  containsValue(\_:) 

Instance Method

# containsValue(\_:)

Checks to see if the target data element’s value is the same as the value parameter or if it contains the value parameter.

macOS

``` source
func containsValue(_ cmpValue: NSObject!) -> Bool
```

## Parameters 

`cmpValue`  

The value to compare with (and search for).

## Return Value

Returns TRUE if the target’s value either matches the given value or if it contains the given value.

## Discussion

This method works just like -containsDataElement: except that it is comparing the value objects directly.

