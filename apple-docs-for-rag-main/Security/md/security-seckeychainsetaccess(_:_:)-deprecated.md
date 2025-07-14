

- Security
-  SecKeychainSetAccess(\_:\_:) Deprecated

Function

# SecKeychainSetAccess(\_:\_:)

Sets the application access for a keychain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainSetAccess(
    _ keychain: SecKeychain?,
    _ access: SecAccess
) -> OSStatus
```

Deprecated

In addition to the ACLs for individual keychain items, the keychain itself has ACLs. However, they are currently unused and this function isn’t implemented.

## Parameters 

`keychain`  

A reference to the keychain for which to set the access. Pass `NULL` to specify the default keychain.

`access`  

An access object of type SecAccess containing access control lists for the keychain. See Access Control Lists for more information about creating an access object.

## Return Value

A result code. See Security Framework Result Codes.

