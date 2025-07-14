

- Security
-  SecKeychainGetUserInteractionAllowed(\_:) Deprecated

Function

# SecKeychainGetUserInteractionAllowed(\_:)

Indicates whether keychain services functions that normally display a user interaction are allowed to do so.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainGetUserInteractionAllowed(_ state: UnsafeMutablePointer) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`state`  

On return, a Boolean value indicating whether user interaction is permitted. If true, user interaction is allowed, and keychain services functions that display a user interface can do so as appropriate.

## Return Value

A result code. See Security Framework Result Codes.

