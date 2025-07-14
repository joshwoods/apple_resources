

- Security
-  SecKeyCreateFromData(\_:\_:\_:) Deprecated

Function

# SecKeyCreateFromData(\_:\_:\_:)

Constructs a SecKeyRef object for a symmetric key.

macOS 10.7–12.0Deprecated

``` source
func SecKeyCreateFromData(
    _ parameters: CFDictionary,
    _ keyData: CFData,
    _ error: UnsafeMutablePointer?>?
) -> SecKey?
```

Deprecated

No longer supported

## Parameters 

`parameters`  

A parameter dictionary that describes the key. See the discussion for details.

`keyData`  

A `CFDataRef` object that contains the raw key data.

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 variable where an error object is stored upon failure. If not `NULL`, the caller is responsible for checking this variable and releasing the resulting object if it exists.

## Return Value

A symmetric key. In Objective-C, call the CFRelease function to free the key’s memory when you are done with it.

## Discussion

The parameters dictionary must contain (at minimum) an entry for the kSecAttrKeyType key with a value of kSecAttrKeyTypeAES or any other key type defined in Key Type Value.

The keys below may be optionally set in the parameters dictionary (with a `CFBooleanRef` value) to override the default key usage values:

- kSecAttrCanEncrypt

- kSecAttrCanDecrypt

- kSecAttrCanWrap

- kSecAttrCanUnwrap

These values default to `true` if no value is specified.

