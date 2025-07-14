

- Security
-  SecKeychainGetPreferenceDomain(\_:) Deprecated

Function

# SecKeychainGetPreferenceDomain(\_:)

Gets the current keychain preference domain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainGetPreferenceDomain(_ domain: UnsafeMutablePointer) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`domain`  

On return, a pointer to the keychain preference domain. See SecPreferencesDomain for possible domain values.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

A preference domain is a set of security-related preferences, such as the default keychain and the current keychain search list. The default preference domain for system daemons (that is, for daemons running in the root session) is the system domain. The default preference domain for all other programs is the user domain. Use the SecKeychainSetPreferenceDomain(_:) function to change the preference domain.

