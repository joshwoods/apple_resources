

- Core Foundation
-  CFSetReleaseCallBack 

Type Alias

# CFSetReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from a set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFSetReleaseCallBack = (CFAllocator?, UnsafeRawPointer?) -> Void
```

## Parameters 

`allocator`  

The set’s allocator.

`value`  

The value being removed from the set.

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

typealias CFSetHashCallBack

Prototype of a callback function called to compute a hash code for a value. Hash codes are used when values are accessed, added, or removed from a collection.

typealias CFSetRetainCallBack

Prototype of a callback function used to retain a value being added to a set.

