

- Security
-  SecTransformCreate(\_:\_:) Deprecated

Function

# SecTransformCreate(\_:\_:)

Creates a transform computation object.

macOS 10.7–13.0Deprecated

``` source
func SecTransformCreate(
    _ name: CFString,
    _ error: UnsafeMutablePointer?>?
) -> SecTransform?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`name`  

The type of transform to create. Use one of the pre-defined transform types or a custom type that you previously registered using SecTransformRegister(_:_:_:).

`error`  

A pointer that the function uses to provide an error object with details if an error occurs. The caller becomes responsible for the object’s memory. Pass `NULL` to ignore the error.

## Return Value

A pointer to a new transform or `NULL` on failure. In Objective-C, call the CFRelease function to free this object’s memory when you are done with it.

