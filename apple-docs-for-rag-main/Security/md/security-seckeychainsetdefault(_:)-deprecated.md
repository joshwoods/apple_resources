

- Security
-  SecKeychainSetDefault(\_:) Deprecated

Function

# SecKeychainSetDefault(\_:)

Sets the default keychain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainSetDefault(_ keychain: SecKeychain?) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`keychain`  

A reference to the keychain you wish to make the default.

## Return Value

A result code. See Security Framework Result Codes. The result code errSecNoSuchKeychain indicates that the specified keychain could not be found. The result code errSecInvalidKeychain indicates that the specified keychain is invalid.

## Discussion

In most cases, your application should not need to set the default keychain, because this is a choice normally made by the user. You may call this function to change where a password or other keychain items are added, but since this is a user choice, you should set the default keychain back to the user specified keychain when you are done.

