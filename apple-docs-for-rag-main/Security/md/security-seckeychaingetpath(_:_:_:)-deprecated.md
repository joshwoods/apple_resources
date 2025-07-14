

- Security
-  SecKeychainGetPath(\_:\_:\_:) Deprecated

Function

# SecKeychainGetPath(\_:\_:\_:)

Determines the path of a keychain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainGetPath(
    _ keychain: SecKeychain?,
    _ ioPathLength: UnsafeMutablePointer,
    _ pathName: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`keychain`  

A reference to a keychain whose path you wish to obtain.

`ioPathLength`  

On entry, a pointer to a variable containing the length (in bytes) of the buffer specified by `pathName`.

On return, the string length of `pathName`, not including the null termination.

`pathName`  

On entry, a pointer to a buffer that you have allocated. On return, the buffer contains POSIX path of the keychain as a null-terminated UTF-8 encoded string. The function returns errSecBufferTooSmall if the provided buffer is too small to hold the string with the null terminator byte.

## Return Value

A result code. See Security Framework Result Codes.

