

- Security
-  SecKeychainLockAll() Deprecated

Function

# SecKeychainLockAll()

Locks all keychains belonging to the current user.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainLockAll() -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Your application should not call this function unless you are responding to a user’s request to lock a keychain. In general, you should leave the keychain unlocked so that the user does not have to unlock it again in another application.

