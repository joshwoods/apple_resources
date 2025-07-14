

- Core Foundation
-  CFSetApplyFunction(\_:\_:\_:) 

Function

# CFSetApplyFunction(\_:\_:\_:)

Calls a function once for each value in a set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetApplyFunction(
    _ theSet: CFSet!,
    _ applier: ((UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void)!,
    _ context: UnsafeMutableRawPointer!
)
```

## Parameters 

`theSet`  

The set to operate upon.

`applier`  

The callback function to call once for each value in the `theSet`. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. The `applier` function must be able to work with all values in `theSet`.

`context`  

A pointer-sized program-defined value, which is passed as the second parameter to the `applier` function, but is otherwise unused by this function.

## Discussion

If `theSet` is mutable, it is unsafe for the `applier` function to change the contents of the collection.

