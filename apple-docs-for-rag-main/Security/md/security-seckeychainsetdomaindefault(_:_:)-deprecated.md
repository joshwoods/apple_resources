

- Security
-  SecKeychainSetDomainDefault(\_:\_:) Deprecated

Function

# SecKeychainSetDomainDefault(\_:\_:)

Sets the default keychain for a specified preference domain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainSetDomainDefault(
    _ domain: SecPreferencesDomain,
    _ keychain: SecKeychain?
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`domain`  

The preference domain for which you wish to set the default keychain. See SecPreferencesDomain for possible domain values.

`keychain`  

A reference to the keychain you wish to set as default in the specified preference domain.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

A preference domain is a set of security-related preferences, such as the default keychain and the current keychain search list. Use this function if you want to set the default keychain for a specific preference domain. Use the SecKeychainSetDefault(_:) function if you want to set the default keychain for the current preference domain. See the SecKeychainSetPreferenceDomain(_:) function for a discussion of current and default preference domains.

