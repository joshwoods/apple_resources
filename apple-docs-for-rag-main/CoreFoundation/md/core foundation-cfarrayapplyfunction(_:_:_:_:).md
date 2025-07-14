

- Core Foundation
-  CFArrayApplyFunction(\_:\_:\_:\_:) 

Function

# CFArrayApplyFunction(\_:\_:\_:\_:)

Calls a function once for each element in range in an array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayApplyFunction(
    _ theArray: CFArray!,
    _ range: CFRange,
    _ applier: ((UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void)!,
    _ context: UnsafeMutableRawPointer!
)
```

## Parameters 

`theArray`  

The array to whose elements to apply the function.

`range`  

The range of values within `theArray` to which to apply the `applier` function. The range must not exceed the bounds of `theArray`. The range may be empty (length `0`).

`applier`  

The callback function to call once for each value in the given range in `theArray`. If there are values in the range that the `applier` function does not expect or cannot properly apply to, the behavior is undefined.

`context`  

A pointer-sized program-defined value, which is passed as the second argument to the `applier` function, but is otherwise unused by this function. If the context is not what is expected by the applier function, the behavior is undefined.

## Discussion

While this function iterates over a mutable collection, it is unsafe for the `applier` function to change the contents of the collection.

