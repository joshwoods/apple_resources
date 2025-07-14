

- Security
-  SecKeychainCopyDefault(\_:) Deprecated

Function

# SecKeychainCopyDefault(\_:)

Retrieves a pointer to the default keychain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainCopyDefault(_ keychain: UnsafeMutablePointer) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`keychain`  

On return, a pointer to the default keychain object. In Objective-C, call the CFRelease function to release this object when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes. The result code errSecNoDefaultKeychain indicates that there is no default keychain.

