

- Security
-  SecTransformCreateFromExternalRepresentation(\_:\_:) Deprecated

Function

# SecTransformCreateFromExternalRepresentation(\_:\_:)

Creates a transform instance from a dictionary of parameters.

macOS 10.7–12.0Deprecated

``` source
func SecTransformCreateFromExternalRepresentation(
    _ dictionary: CFDictionary,
    _ error: UnsafeMutablePointer?>?
) -> SecTransform?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`dictionary`  

The dictionary of parameters.

`error`  

An optional pointer to a CFErrorRef. This value is set if an error occurred. If not NULL the caller is responsible for releasing the CFErrorRef.

## Return Value

A pointer to a SecTransformRef object. You must release the object with CFRelease when you are done with it. A NULL will be returned if an error occurred during initialization, and if the error parameter is non-null, it contains the specific error data.

