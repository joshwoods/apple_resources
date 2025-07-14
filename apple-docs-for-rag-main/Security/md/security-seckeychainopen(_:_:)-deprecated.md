

- Security
-  SecKeychainOpen(\_:\_:) Deprecated

Function

# SecKeychainOpen(\_:\_:)

Opens a keychain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainOpen(
    _ pathName: UnsafePointer,
    _ keychain: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`pathName`  

A constant character string representing the POSIX path to the keychain to open.

`keychain`  

On return, a pointer to the keychain object. You must call the `CFRelease` function to release this object when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Use this function to retrieve a pointer to a keychain object given the path of the keychain. You don’t need to close the keychain, but do release the memory that the pointer occupies when you are finished with it.

