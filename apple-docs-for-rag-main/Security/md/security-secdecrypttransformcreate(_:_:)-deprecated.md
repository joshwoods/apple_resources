

- Security
-  SecDecryptTransformCreate(\_:\_:) Deprecated

Function

# SecDecryptTransformCreate(\_:\_:)

Creates a decryption transform object.

macOS 10.7–13.0Deprecated

``` source
func SecDecryptTransformCreate(
    _ keyRef: SecKey,
    _ error: UnsafeMutablePointer?>?
) -> SecTransform
```

Deprecated

SecTransform is no longer supported

## Parameters 

`keyRef`  

The key for the operation

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8. This pointer will be set if an error occurred. This value may be `NULL` if you do not want an error returned.

## Return Value

A pointer to a new transform or `nil` on error. In Objective-C, call the CFRelease function to free this object’s memory when you are done with it.

## Discussion

This function creates a transform which decrypts data.

