

- Security
-  SecEncodeTransformCreate(\_:\_:) Deprecated

Function

# SecEncodeTransformCreate(\_:\_:)

Creates an encode transform object.

macOS 10.7–13.0Deprecated

``` source
func SecEncodeTransformCreate(
    _ encodeType: CFTypeRef,
    _ error: UnsafeMutablePointer?>?
) -> SecTransform?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`encodeType`  

The type of digest to compute. You may pass `NULL` for this parameter, in which case an appropriate algorithm will be chosen for you. See `Encoding Types` for a list of valid values.

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8. This pointer will be set if an error occurred. This value may be `nil` if you do not want an error returned.

## Return Value

A pointer to a new transform or `NULL` on error. In Objective-C, call the CFRelease function to free this object’s memory when you are done with it.

## Discussion

This function creates a transform which computes an encode.

