

- Core Foundation
-  CFDictionaryApplyFunction(\_:\_:\_:) 

Function

# CFDictionaryApplyFunction(\_:\_:\_:)

Calls a function once for each key-value pair in a dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDictionaryApplyFunction(
    _ theDict: CFDictionary!,
    _ applier: ((UnsafeRawPointer?, UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void)!,
    _ context: UnsafeMutableRawPointer!
)
```

## Parameters 

`theDict`  

The dictionary to operate upon.

`applier`  

The callback function to call once for each key-value pair in `theDict`. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. If there are keys or values which the `applier` function does not expect or cannot properly apply to, the behavior is undefined.

`context`  

A pointer-sized program-defined value, which is passed as the third parameter to the applier function, but is otherwise unused by this function. The value must be appropriate for the `applier` function.

## Discussion

If this function iterates over a mutable collection, it is unsafe for the `applier` function to change the contents of the collection.

