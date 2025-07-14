

- Core Foundation
-  CFBagHashCallBack 

Type Alias

# CFBagHashCallBack

Prototype of a callback function invoked to compute a hash code for a value. Hash codes are used when values are accessed, added, or removed from a collection.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFBagHashCallBack = (UnsafeRawPointer?) -> CFHashCode
```

## Parameters 

`value`  

The value used to compute the hash code.

## Return Value

An integer that can be used as a table address in a hash table structure.

## Discussion

This callback is passed to CFBagCreate(_:_:_:_:) in a CFBagCallBacks structure.

## See Also

### Callbacks

typealias CFBagApplierFunction

Prototype of a callback function that may be applied to every value in a bag.

typealias CFBagCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value in a bag.

typealias CFBagEqualCallBack

Prototype of a callback function used to determine if two values in a bag are equal.

typealias CFBagReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from a bag.

typealias CFBagRetainCallBack

Prototype of a callback function used to retain a value being added to a bag.

