

- Security
-  SecKeyUnwrapSymmetric(\_:\_:\_:\_:) Deprecated

Function

# SecKeyUnwrapSymmetric(\_:\_:\_:\_:)

Unwraps a wrapped symmetric key.

macOS 10.7–12.0Deprecated

``` source
func SecKeyUnwrapSymmetric(
    _ keyToUnwrap: UnsafeMutablePointer?>,
    _ unwrappingKey: SecKey,
    _ parameters: CFDictionary,
    _ error: UnsafeMutablePointer?>?
) -> SecKey?
```

Deprecated

No longer supported

## Parameters 

`keyToUnwrap`  

The wrapped key to unwrap.

`unwrappingKey`  

The key that must be used to unwrap `keyToUnwrap`.

`parameters`  

A parameter list for the unwrapping process. This is usually either an empty dictionary or a dictionary containing a value for kSecAttrSalt.

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 variable where an error object is stored upon failure. If not `NULL`, the caller is responsible for checking this variable and releasing the resulting object if it exists.

## Return Value

The unwrapped key, or `NULL` on failure. In Objective-C, call the CFRelease function to free the key’s memory when you are done with it.

