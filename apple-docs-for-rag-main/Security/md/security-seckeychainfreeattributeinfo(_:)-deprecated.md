

- Security
-  SecKeychainFreeAttributeInfo(\_:) Deprecated

Function

# SecKeychainFreeAttributeInfo(\_:)

Releases the memory acquired by calling the `SecKeychainAttributeInfoForItemID` function.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainFreeAttributeInfo(_ info: UnsafeMutablePointer) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`info`  

A pointer to the keychain attribute information to release.

## Return Value

A result code. See Security Framework Result Codes.

