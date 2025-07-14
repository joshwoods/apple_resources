

- Security
-  SecDigestTransformCreate(\_:\_:\_:) Deprecated

Function

# SecDigestTransformCreate(\_:\_:\_:)

Creates a digest transform object.

macOS 10.7–13.0Deprecated

``` source
func SecDigestTransformCreate(
    _ digestType: CFTypeRef?,
    _ digestLength: CFIndex,
    _ error: UnsafeMutablePointer?>?
) -> SecTransform
```

Deprecated

SecTransform is no longer supported

## Parameters 

`digestType`  

The type of digest to compute. You may pass `NULL` for this parameter, in which case an appropriate algorithm will be chosen for you. Otherwise, use one of the values listed in `Digest Constants`.

`digestLength`  

The desired digest length. Note that certain algorithms may only support certain sizes. You may pass `0` for this parameter, in which case an appropriate length will be chosen for you.

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8. This pointer will be set if an error occurred. This value may be `nil` if you do not want an error returned.

## Return Value

A pointer to a new transform or `NULL` on error. In Objective-C, call the CFRelease function to free this object’s memory when you are done with it.

## Discussion

This function creates a transform which computes a cryptographic digest.

