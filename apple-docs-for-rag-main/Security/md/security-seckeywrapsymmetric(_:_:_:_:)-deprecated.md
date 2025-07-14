

- Security
-  SecKeyWrapSymmetric(\_:\_:\_:\_:) Deprecated

Function

# SecKeyWrapSymmetric(\_:\_:\_:\_:)

Wraps a symmetric key with another key.

macOS 10.7–12.0Deprecated

``` source
func SecKeyWrapSymmetric(
    _ keyToWrap: SecKey,
    _ wrappingKey: SecKey,
    _ parameters: CFDictionary,
    _ error: UnsafeMutablePointer?>?
) -> CFData?
```

Deprecated

No longer supported

## Parameters 

`keyToWrap`  

The key to wrap.

`wrappingKey`  

The key to use when wrapping `keyToWrap`.

`parameters`  

A parameter list for the unwrapping process. This is usually either an empty dictionary or a dictionary containing a value for kSecAttrSalt.

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 variable where an error object is stored upon failure. If not `NULL`, the caller is responsible for checking this variable and releasing the resulting object if it exists.

## Return Value

The wrapped key, or `NULL` on error. In Objective-C, call the CFRelease function to free the data’s memory when you are done with it.

