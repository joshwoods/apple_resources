

- Core Foundation
-  CFSetHashCallBack 

Type Alias

# CFSetHashCallBack

Prototype of a callback function called to compute a hash code for a value. Hash codes are used when values are accessed, added, or removed from a collection.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFSetHashCallBack = (UnsafeRawPointer?) -> CFHashCode
```

## Parameters 

`value`  

The value used to compute the hash code.

## Return Value

An integer that can be used as a table address in a hash table structure.

## Discussion

This callback is passed to CFSetCreate(_:_:_:_:) in a CFSetCallBacks structure.

## See Also

### Callbacks

typealias CFSetApplierFunction

Prototype of a callback function that may be applied to every value in a set.

typealias CFSetCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value in a set.

typealias CFSetEqualCallBack

Prototype of a callback function used to determine if two values in a set are equal.

typealias CFSetReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from a set.

typealias CFSetRetainCallBack

Prototype of a callback function used to retain a value being added to a set.

