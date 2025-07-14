

- Security
-  SecKeychainCopyAccess(\_:\_:) Deprecated

Function

# SecKeychainCopyAccess(\_:\_:)

Retrieves the application access of a keychain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainCopyAccess(
    _ keychain: SecKeychain?,
    _ access: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

This function is not implemented and returns an errSecUnimplemented error code if called.

## Parameters 

`keychain`  

A reference to the keychain from which to copy the access object. Pass `NULL` to specify the default keychain.

`access`  

A pointer to an access object. On return, this points to the access object of the specified keychain.

## Return Value

A result code. See Security Framework Result Codes.

