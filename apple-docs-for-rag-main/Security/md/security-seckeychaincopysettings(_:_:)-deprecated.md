

- Security
-  SecKeychainCopySettings(\_:\_:) Deprecated

Function

# SecKeychainCopySettings(\_:\_:)

Obtains a keychain’s settings.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainCopySettings(
    _ keychain: SecKeychain?,
    _ outSettings: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`keychain`  

A reference to the keychain from which to copy its settings.

`outSettings`  

On return, a pointer to a keychain settings structure. Since this structure is versioned, you must allocate the memory for it and fill in the version of the structure before passing it to the function.

## Return Value

A result code. See Security Framework Result Codes.

