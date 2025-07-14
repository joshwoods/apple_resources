

- Security
-  SecKeychainCopyDomainSearchList(\_:\_:) Deprecated

Function

# SecKeychainCopyDomainSearchList(\_:\_:)

Retrieves the keychain search list for a specified preference domain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainCopyDomainSearchList(
    _ domain: SecPreferencesDomain,
    _ searchList: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`domain`  

The preference domain from which you wish to retrieve the keychain search list. See SecPreferencesDomain for possible domain values.

`searchList`  

On return, a pointer to the keychain search list of the specified preference domain.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

A preference domain is a set of security-related preferences, such as the default keychain and the current keychain search list. Use this function if you want to retrieve the keychain search list for a specific preference domain. Use the SecKeychainCopySearchList(_:) function if you want the keychain search list for the current preference domain. See the SecKeychainSetPreferenceDomain(_:) function for a discussion of current and default preference domains.

