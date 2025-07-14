

- Security
-  SecSignTransformCreate(\_:\_:) Deprecated

Function

# SecSignTransformCreate(\_:\_:)

Creates a signing transform object.

macOS 10.7–13.0Deprecated

``` source
func SecSignTransformCreate(
    _ key: SecKey,
    _ error: UnsafeMutablePointer?>?
) -> SecTransform?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`key`  

A SecKey with the private key used for signing.

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8. This pointer will be set if an error occurred. This value may be `NULL` if you do not want an error returned.

## Return Value

A pointer to a new transform or `NULL` on error. In Objective-C, call the CFRelease function to free this object’s memory when you are done with it.

## Discussion

This function creates a transform which computes a cryptographic signature. The kSecInputIsAttributeName attribute defaults to kSecInputIsPlainText, and the kSecDigestTypeAttribute and kSecDigestLengthAttribute attributes default to something appropriate for the type of key you have supplied.

