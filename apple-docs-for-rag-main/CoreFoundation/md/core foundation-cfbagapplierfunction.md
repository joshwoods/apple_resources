

- Core Foundation
-  CFBagApplierFunction 

Type Alias

# CFBagApplierFunction

Prototype of a callback function that may be applied to every value in a bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFBagApplierFunction = (UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`value`  

The current value in a bag.

`context`  

The program-defined context parameter given to the apply function.

## Discussion

This callback is passed to the CFBagApplyFunction(_:_:_:) function which iterates over the values in a bag and applies the behavior defined in the applier function to each value in a bag.

## See Also

### Callbacks

typealias CFBagCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value in a bag.

typealias CFBagEqualCallBack

Prototype of a callback function used to determine if two values in a bag are equal.

typealias CFBagHashCallBack

Prototype of a callback function invoked to compute a hash code for a value. Hash codes are used when values are accessed, added, or removed from a collection.

typealias CFBagReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from a bag.

typealias CFBagRetainCallBack

Prototype of a callback function used to retain a value being added to a bag.

