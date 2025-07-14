

- Core Foundation
-  CFArrayApplierFunction 

Type Alias

# CFArrayApplierFunction

Prototype of a callback function that may be applied to every value in an array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFArrayApplierFunction = (UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`value`  

The current value in an array.

`context`  

The program-defined context parameter given to the applier function.

## Discussion

This callback is passed to the CFArrayApplyFunction(_:_:_:_:) function, which iterates over the values in an array and applies the behavior defined in the applier function to each value in an array.

## See Also

### Callbacks

typealias CFArrayCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value in an array.

typealias CFArrayEqualCallBack

Prototype of a callback function used to determine if two values in an array are equal.

typealias CFArrayReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from an array.

typealias CFArrayRetainCallBack

Prototype of a callback function used to retain a value being added to an array.

