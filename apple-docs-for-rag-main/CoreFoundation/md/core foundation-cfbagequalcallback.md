

- Core Foundation
-  CFBagEqualCallBack 

Type Alias

# CFBagEqualCallBack

Prototype of a callback function used to determine if two values in a bag are equal.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFBagEqualCallBack = (UnsafeRawPointer?, UnsafeRawPointer?) -> DarwinBoolean
```

## Parameters 

`value1`  

A value in the bag.

`value2`  

Another value in the bag.

## Return Value

`true` if `value1` and `value2` are equal, `false` otherwise.

## Discussion

This callback is passed to CFBagCreate(_:_:_:_:) in a CFBagCallBacks structure.

## See Also

### Callbacks

typealias CFBagApplierFunction

Prototype of a callback function that may be applied to every value in a bag.

typealias CFBagCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value in a bag.

typealias CFBagHashCallBack

Prototype of a callback function invoked to compute a hash code for a value. Hash codes are used when values are accessed, added, or removed from a collection.

typealias CFBagReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from a bag.

typealias CFBagRetainCallBack

Prototype of a callback function used to retain a value being added to a bag.

