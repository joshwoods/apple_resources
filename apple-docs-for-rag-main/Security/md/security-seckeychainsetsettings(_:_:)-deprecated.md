

- Security
-  SecKeychainSetSettings(\_:\_:) Deprecated

Function

# SecKeychainSetSettings(\_:\_:)

Changes the settings of a keychain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainSetSettings(
    _ keychain: SecKeychain?,
    _ newSettings: UnsafePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`keychain`  

A reference to a keychain whose settings you wish to change. Pass `NULL` to change the settings of the default keychain.

`newSettings`  

A pointer to a keychain settings structure that defines whether the keychain locks when sleeping, or locks after a set time period of inactivity.

## Return Value

A result code. See Security Framework Result Codes.

