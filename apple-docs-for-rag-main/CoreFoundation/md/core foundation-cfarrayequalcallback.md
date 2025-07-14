

- Core Foundation
-  CFArrayEqualCallBack 

Type Alias

# CFArrayEqualCallBack

Prototype of a callback function used to determine if two values in an array are equal.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFArrayEqualCallBack = (UnsafeRawPointer?, UnsafeRawPointer?) -> DarwinBoolean
```

## Parameters 

`value1`  

A value in an array to be compared with `value2` for equality.

`value2`  

A value in an array to be compared with `value1` for equality.

## Return Value

`true` if `value1` and `value2` are equal, `false` otherwise.

## Discussion

This callback is passed to CFArrayCreate(_:_:_:_:) in a CFArrayCallBacks structure.

## See Also

### Callbacks

typealias CFArrayApplierFunction

Prototype of a callback function that may be applied to every value in an array.

typealias CFArrayCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value in an array.

typealias CFArrayReleaseCallBack

Prototype of a callback function used to release a value before it’s removed from an array.

typealias CFArrayRetainCallBack

Prototype of a callback function used to retain a value being added to an array.

