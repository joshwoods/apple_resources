

- Security
-  SecKeyDeriveFromPassword(\_:\_:\_:) Deprecated

Function

# SecKeyDeriveFromPassword(\_:\_:\_:)

Returns a key object in which the key data is derived from a password.

macOS 10.7–12.0Deprecated

``` source
func SecKeyDeriveFromPassword(
    _ password: CFString,
    _ parameters: CFDictionary,
    _ error: UnsafeMutablePointer?>?
) -> SecKey?
```

Deprecated

No longer supported

## Parameters 

`password`  

The password from which the key should be derived.

`parameters`  

A set of parameters for deriving the password.

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 variable where an error object is stored upon failure. If not `NULL`, the caller is responsible for checking this variable and releasing the resulting object if it exists.

## Return Value

The derived key object, or `NULL` on error. In Objective-C, call the CFRelease function to free the key’s memory when you are done with it.

## Discussion

The parameters dictionary must contain at least the following keys:

- kSecKeyKeyType—the type of symmetric key to generate.

- kSecAttrSalt—a `CFDataRef` object containing the salt value that is mixed into the pseudorandom rounds.

The parameters dictionary may contain the following optional keys:

- kSecAttrPRF - the algorithm to use for the pseudorandom-function.

If zero, this defaults to kSecAttrPRFHmacAlgSHA1. For a list of possible values, see `kSecAttrPRF Value Constants`.

- kSecAttrRounds—the number of times to call the pseudorandom function. If zero, the count is computed so that computation will take 1/10 of a second (on average).

- kSecAttrKeySizeInBits—a `CFNumberRef` value containing the requested key size in bits. The key size must be valid for the key type. Defaults to 128 if not provided.

