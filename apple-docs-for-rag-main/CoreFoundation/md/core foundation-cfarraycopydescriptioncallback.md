

- Core Foundation
-  CFArrayCopyDescriptionCallBack 

Type Alias

# CFArrayCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value in an array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFArrayCopyDescriptionCallBack = (UnsafeRawPointer?) -> Unmanaged?
```

## Parameters 

`value`  

The value to be described.

## Return Value

A textual description of `value`. The caller is responsible for releasing this object.

## Discussion

This callback is passed to CFArrayCreate(_:_:_:_:) in a CFArrayCallBacks structure. This callback is used by the CFCopyDescription(_:) function.

## See Also

### Callbacks

typealias CFArrayApplierFunction

Prototype of a callback function that may be applied to every value in an array.

typealias CFArrayEqualCallBack

Prototype of a callback function used to determine if two values in an array are equal.

typealias CFArrayReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from an array.

typealias CFArrayRetainCallBack

Prototype of a callback function used to retain a value being added to an array.

