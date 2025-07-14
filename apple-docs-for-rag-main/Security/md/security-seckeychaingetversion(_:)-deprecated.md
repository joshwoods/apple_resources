

- Security
-  SecKeychainGetVersion(\_:) Deprecated

Function

# SecKeychainGetVersion(\_:)

Determines the version of keychain services installed on the user’s system.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainGetVersion(_ returnVers: UnsafeMutablePointer) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`returnVers`  

On return, a pointer to the version number of keychain services installed on the current system. See `Keychain Settings Version` for a list of values.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Your application can call the SecKeychainGetVersion(_:) function to find out which version of keychain services is installed on the user’s system.

