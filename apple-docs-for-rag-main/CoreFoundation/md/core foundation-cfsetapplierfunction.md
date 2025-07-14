

- Core Foundation
-  CFSetApplierFunction 

Type Alias

# CFSetApplierFunction

Prototype of a callback function that may be applied to every value in a set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFSetApplierFunction = (UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`value`  

The current value in a set.

`context`  

The program-defined context parameter given to the apply function.

## Discussion

This callback is passed to the CFSetApplyFunction(_:_:_:) function which iterates over the values in a set and applies the behavior defined in the applier function to each value in a set.

## See Also

### Callbacks

typealias CFSetCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value in a set.

typealias CFSetEqualCallBack

Prototype of a callback function used to determine if two values in a set are equal.

typealias CFSetHashCallBack

Prototype of a callback function called to compute a hash code for a value. Hash codes are used when values are accessed, added, or removed from a collection.

typealias CFSetReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from a set.

typealias CFSetRetainCallBack

Prototype of a callback function used to retain a value being added to a set.

