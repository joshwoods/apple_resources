

- Security
-  SecKeychainCopyDomainDefault(\_:\_:) Deprecated

Function

# SecKeychainCopyDomainDefault(\_:\_:)

Retrieves the default keychain from a specified preference domain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainCopyDomainDefault(
    _ domain: SecPreferencesDomain,
    _ keychain: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`domain`  

The preference domain from which you wish to retrieve the default keychain. See SecPreferencesDomain for possible domain values.

`keychain`  

On return, a pointer to the keychain object of the default keychain in the specified preference domain.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

A preference domain is a set of security-related preferences, such as the default keychain and the current keychain search list. Use this function if you want to retrieve the default keychain for a specific preference domain. Use the SecKeychainCopyDefault(_:) function if you want the default keychain for the current preference domain. See the SecKeychainSetPreferenceDomain(_:) function for a discussion of current and default preference domains.

