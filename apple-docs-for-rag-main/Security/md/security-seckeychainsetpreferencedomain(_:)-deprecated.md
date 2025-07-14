

- Security
-  SecKeychainSetPreferenceDomain(\_:) Deprecated

Function

# SecKeychainSetPreferenceDomain(\_:)

Sets the keychain preference domain.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainSetPreferenceDomain(_ domain: SecPreferencesDomain) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`domain`  

The keychain preference domain to set. See SecPreferencesDomain for possible domain values.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

A preference domain is a set of security-related preferences, such as the default keychain and the current keychain search list. The default preference domain for system daemons (that is, for daemons running in the root session) is the system domain. The default preference domain for all other programs is the user domain.

This function changes the preference domain for all subsequent function calls; for example, if you change from the system domain to the user domain and then call SecKeychainLock(_:) specifying `NULL` for the keychain, the function locks the default system keychain rather than the default user keychain. You might want to use this function, for example, when launching a system daemon from a user session so that the daemon uses system preferences rather than user preferences.

