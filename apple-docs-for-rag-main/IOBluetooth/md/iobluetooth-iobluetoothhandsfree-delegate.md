

- IOBluetooth
- IOBluetoothHandsFree
-  delegate 

Instance Property

# delegate

Return the delegate

macOS 10.7+

``` source
unowned(unsafe) var delegate: (any IOBluetoothHandsFreeDelegate)! { get set }
```

## Return Value

The delegate for the hands free object or nil if it doesn’t have a delegate.

## Discussion

Returns the hands free object’s delegate.

