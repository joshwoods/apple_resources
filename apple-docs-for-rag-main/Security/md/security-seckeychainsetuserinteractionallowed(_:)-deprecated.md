

- Security
-  SecKeychainSetUserInteractionAllowed(\_:) Deprecated

Function

# SecKeychainSetUserInteractionAllowed(\_:)

Enables or disables the user interface for keychain services functions that automatically display a user interface.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainSetUserInteractionAllowed(_ state: Bool) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`state`  

A flag that indicates whether the keychain services will display a user interface. If you pass true, user interaction is allowed. This is the default value. If false, keychain services functions that normally display a user interface will instead return an error.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Certain keychain services functions that require the presence of a keychain automatically display a *Keychain Not Found* dialog if there is none. Functions that require the keychain to be unlocked automatically display the *Unlock Keychain* dialog. The SecKeychainSetUserInteractionAllowed(_:) function enables you to control whether these functions display a user interface. By default, user interaction is permitted.

If you are writing an application that must run unattended on a server, you may wish to disable the user interface so that any subsequent keychain calls that normally bring up the unlock UI will instead return immediately with an errSecInteractionRequired result). In this case you must programmatically create a keychain or unlock the keychain when necessary.

### Special Considerations

If you disable user interaction before calling a Keychain Services function, be sure to reenable it when you are finished. Failure to reenable user interaction will affect other clients of the Keychain Services.

