

- Core Foundation
-  CFBagRetainCallBack 

Type Alias

# CFBagRetainCallBack

Prototype of a callback function used to retain a value being added to a bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFBagRetainCallBack = (CFAllocator?, UnsafeRawPointer?) -> UnsafeRawPointer?
```

## Parameters 

`allocator`  

The bag’s allocator.

`value`  

The value being added to the bag.

## Return Value

The value to store in the bag, which is usually the `value` parameter passed to this callback, but may be a different value if a different value should be stored in the collection.

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

typealias CFBagHashCallBack

Prototype of a callback function invoked to compute a hash code for a value. Hash codes are used when values are accessed, added, or removed from a collection.

typealias CFBagReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from a bag.

