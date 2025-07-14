

- Security
-  SecKeychainSetDomainSearchList(\_:\_:) Deprecated

Function

# SecKeychainSetDomainSearchList(\_:\_:)

Sets the keychain search list for a specified preference domain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainSetDomainSearchList(
    _ domain: SecPreferencesDomain,
    _ searchList: CFArray
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`domain`  

The preference domain for which you wish to set the default keychain search list. See SecPreferencesDomainfor possible domain values.

`searchList`  

A pointer to a keychain search list to set in the preference domain.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

A preference domain is a set of security-related preferences, such as the default keychain and the current keychain search list. Use this function if you want to set the keychain search list for a specific preference domain. Use the SecKeychainSetSearchList(_:) function if you want to set the keychain search list for the current preference domain. See the SecKeychainSetPreferenceDomain(_:) function for a discussion of current and default preference domains.

