

- Security
-  SecTransformRegister(\_:\_:\_:) Deprecated

Function

# SecTransformRegister(\_:\_:\_:)

Registers a custom transform.

macOS 10.7–13.0Deprecated

``` source
func SecTransformRegister(
    _ uniqueName: CFString,
    _ createTransformFunction: SecTransformCreateFP,
    _ error: UnsafeMutablePointer?>?
) -> Bool
```

Deprecated

SecTransform is no longer supported

## Parameters 

`uniqueName`  

A unique name for this custom transform. It is recommended that a reverse DNS name be used for the name of your custom transform

`createTransformFunction`  

A SecTransformCreateFP function pointer. The function must return a SecTransformInstanceBlock block. Call block_copy on this block before returning it. Failure to do so results in undefined behavior.

`error`  

A pointer that the function uses to provide an error object with details if an error occurs. The caller becomes responsible for the object’s memory. Pass `NULL` to ignore the error.

## Return Value

A Boolean that is set to true if the custom transform was registered and false otherwise

