

- Core Foundation
-  CFSetCopyDescriptionCallBack 

Type Alias

# CFSetCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value in a set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFSetCopyDescriptionCallBack = (UnsafeRawPointer?) -> Unmanaged?
```

## Parameters 

`value`  

The value to be described.

## Return Value

A textual description of `value`. The caller is responsible for releasing this object.

## Discussion

This callback is passed to CFSetCreate(_:_:_:_:) in a CFSetCallBacks structure. This callback is used by the CFCopyDescription(_:) function.

## See Also

### Callbacks

typealias CFSetApplierFunction

Prototype of a callback function that may be applied to every value in a set.

typealias CFSetEqualCallBack

Prototype of a callback function used to determine if two values in a set are equal.

typealias CFSetHashCallBack

Prototype of a callback function called to compute a hash code for a value. Hash codes are used when values are accessed, added, or removed from a collection.

typealias CFSetReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from a set.

typealias CFSetRetainCallBack

Prototype of a callback function used to retain a value being added to a set.

