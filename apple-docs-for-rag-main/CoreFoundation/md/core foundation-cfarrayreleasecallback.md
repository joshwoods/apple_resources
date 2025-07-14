

- Core Foundation
-  CFArrayReleaseCallBack 

Type Alias

# CFArrayReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from an array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFArrayReleaseCallBack = (CFAllocator?, UnsafeRawPointer?) -> Void
```

## Parameters 

`allocator`  

The array’s allocator.

`value`  

The value being removed from an array.

## Discussion

This callback is passed to CFArrayCreate(_:_:_:_:) in a CFArrayCallBacks structure.

## See Also

### Callbacks

typealias CFArrayApplierFunction

Prototype of a callback function that may be applied to every value in an array.

typealias CFArrayCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value in an array.

typealias CFArrayEqualCallBack

Prototype of a callback function used to determine if two values in an array are equal.

typealias CFArrayRetainCallBack

Prototype of a callback function used to retain a value being added to an array.

