

- Core Foundation
-  CFSetRetainCallBack 

Type Alias

# CFSetRetainCallBack

Prototype of a callback function used to retain a value being added to a set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFSetRetainCallBack = (CFAllocator?, UnsafeRawPointer?) -> UnsafeRawPointer?
```

## Parameters 

`allocator`  

The set’s allocator.

`value`  

The value being added to the set.

## Return Value

The value to store in the set, which is usually the `value` parameter passed to this callback, but may be a different value if a different value should be stored in the collection.

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

typealias CFSetReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from a set.

