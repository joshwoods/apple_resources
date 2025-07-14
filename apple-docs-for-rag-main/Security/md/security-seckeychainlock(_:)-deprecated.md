

- Security
-  SecKeychainLock(\_:) Deprecated

Function

# SecKeychainLock(\_:)

Locks a keychain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainLock(_ keychain: SecKeychain?) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`keychain`  

A reference to the keychain to lock. Pass `NULL` to lock the default keychain.

## Return Value

A result code. See Security Framework Result Codes. The result code errSecNoSuchKeychain indicates that specified keychain could not be found. The result code errSecInvalidKeychain indicates that the specified keychain is invalid.

## Discussion

Your application should not call this function unless you are responding to a user’s request to lock a keychain. In general, you should leave the keychain unlocked so that the user does not have to unlock it again in another application.

